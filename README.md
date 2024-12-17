# Uncommon TailwindCSS Bugs

This repository demonstrates two uncommon bugs that can occur when using Tailwind CSS:

1. **Using `@apply` within styled-components:**  Tailwind's `@apply` directive doesn't work directly within styled-components template literals because styled-components processes CSS differently.
2. **Dynamic class names with potential errors:** If you generate Tailwind class names dynamically, make sure the resulting string is always a valid Tailwind class. Otherwise, you'll get unexpected results.

## Bug 1: styled-components and @apply

The `SomeTailwind.js` file shows an attempt to use `@apply` within a styled-components template literal. This will lead to an error or unexpected behavior.

## Bug 2: Dynamic Class Names

The solution for the second bug involves robust validation of dynamically generated class names before they're applied. This prevents potential runtime errors and ensures the application of valid Tailwind classes.

## Solutions

The `SomeTailwindSolution.js` file demonstrates the correct way to use Tailwind with styled-components and provides a better way to handle dynamic class names.  See the comments in the file for a detailed explanation.