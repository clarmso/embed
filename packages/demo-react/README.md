# React App Demo

Typeform can be embedded in react apps.

**Note:** We recommend using `@typeform/embed-react`, it will be rady soon :)

You can use the `@typeform/embed` directly in react apps:

```javascript
import { createWidget } from "@typeform/embed";
import "@typeform/embed/build/css/widget.css"; // import necessary CSS

const MyTypeformEmbed = () => {
  const container = useRef();

  useEffect(() => {
    createWidget("<form id>", { container: container.current });
  }, []);

  return <div ref={container} />;
};
```

Use `yarn start` to run the demo in browser: http://localhost:8080
