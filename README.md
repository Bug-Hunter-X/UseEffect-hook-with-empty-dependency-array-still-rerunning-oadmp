# React useEffect Hook Unexpected Rerun

This repository demonstrates a common issue with the React `useEffect` hook where an effect with an empty dependency array still reruns unexpectedly on every render. This often stems from a missing dependency or an unintentional side effect.

## Problem

The `useEffect` hook, despite having an empty dependency array (`[]`), should only run once after the initial render. However, in this example, the console log shows it runs multiple times.

## Solution

The solution involves carefully reviewing the `useEffect`'s dependencies and adding any state variables or props it directly or indirectly depends on to the dependency array.

## How to run

1. Clone this repo
2. `npm install`
3. `npm start`