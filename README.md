# Tailwind CSS @apply Directive with Undefined Class

This repository demonstrates a common but often subtle error in Tailwind CSS: using the `@apply` directive with a class that hasn't been defined in your Tailwind configuration.

## The Bug

The `@apply` directive is a powerful feature, but it can lead to hard-to-debug issues if you accidentally reference a class that doesn't exist. The error won't always throw a clear exception; it might simply result in unexpected styling or no styling at all.

## The Solution

The solution is simple: double-check your Tailwind configuration and ensure that all classes used with `@apply` are defined.  Also consider using the `purge` (or `content`) option in your Tailwind config to ensure only used classes are included in your production build, preventing this type of error.