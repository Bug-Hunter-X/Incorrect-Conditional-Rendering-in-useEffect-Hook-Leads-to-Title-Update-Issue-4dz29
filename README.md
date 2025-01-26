# React useEffect Conditional Rendering Bug

This repository demonstrates a common bug in React applications involving incorrect conditional rendering logic within the `useEffect` hook. The bug causes unexpected behavior in updating the document title based on a counter value.

## Bug Description

A React component uses the `useState` hook to manage a counter. The `useEffect` hook attempts to update the document title based on the counter's value. However, due to a flawed conditional check (`if (count > 0)`), the title is not updated when the counter is 0, leading to an incorrect title display.

## Solution

The solution involves removing the unnecessary conditional check. The `useEffect` hook should update the document title regardless of the counter's value, ensuring the title accurately reflects the current count at all times.