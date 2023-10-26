# Class 28 Notes

## Reading

### useEffect hook

What is the main intended use case for the useEffect hook?

- The useEffect hook is primarily intended to perform side effects in functional components. Side effects are operations that don't involve rendering UI but are essential for other purposes.

How does the effect’s logic interact with the component?

- The useEffect hook runs the provided effect function after the component's render has been committed to the screen, ensuring that it doesn't block the visual updates. Depending on its dependencies (provided in the second argument), the effect can be executed after every render or only when certain values have changed.

What is the importance of the return value from the effect’s logic function?

- The return value of the effect's logic function (when provided) is a cleanup function. This function is used to perform any necessary cleanup before the component is unmounted or before re-running the effect due to changes in its dependencies. Cleanup is essential to avoid potential memory leaks, remove event listeners, or cancel any subscriptions or timers.
