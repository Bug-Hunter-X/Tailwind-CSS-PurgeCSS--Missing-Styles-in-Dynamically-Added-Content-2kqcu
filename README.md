# Tailwind CSS PurgeCSS Bug: Missing Styles in Dynamically Added Content

This repository demonstrates a common issue encountered when using Tailwind CSS with dynamically generated content.  The problem arises from Tailwind's PurgeCSS functionality failing to include styles for classes added to the DOM after the initial page render.

## Problem

When content is added dynamically using JavaScript, the PurgeCSS optimization process (which removes unused CSS classes to reduce bundle size) may miss the classes used in that dynamic content. This leads to missing styles and improperly rendered elements.

## Solution

The solution typically involves configuring PurgeCSS to correctly identify and retain styles for the dynamically added content.  This is usually done by adding the appropriate configuration options to your Tailwind CSS setup or using a different strategy for including styles.

This example showcases a simple HTML structure, where we add a button to the DOM.  The `dynamic-content-bug.html` file illustrates the problem of missing styles, while `dynamic-content-solution.html` demonstrates a solution.