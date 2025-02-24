# useOnScrollAt Hook

A custom React hook that triggers callbacks when a specific DOM element becomes visible or hidden based on scroll position.

## 📦 Installation

```bash
npm install react
```

## 🚀 Usage

```tsx
import { useOnScrollAt } from "./useOnScrollAt";

const MyComponent = () => {
  useOnScrollAt(
    "my-element",
    () => console.log("Element is visible"),
    () => console.log("Element is hidden")
  );

  return (
    <div>
      <div style={{ height: "150vh" }}>Scroll down</div>
      <div id="my-element">Watch me!</div>
      <div style={{ height: "150vh" }}></div>
    </div>
  );
};
```

## ⚙️ API

```tsx
useOnScrollAt(
  elementId: string,     // The ID of the target DOM element
  onVisible: () => void, // Callback when element is visible
  onHidden: () => void   // Callback when element is hidden
);
```
