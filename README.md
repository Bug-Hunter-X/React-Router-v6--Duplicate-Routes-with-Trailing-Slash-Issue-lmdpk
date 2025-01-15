# React Router v6 Duplicate Route Bug

This repository demonstrates a common issue in React Router v6 related to duplicate routes, specifically when one route has a trailing slash and the other does not.

## Problem

Defining two routes with the same path, differing only by a trailing slash, leads to unexpected behavior. In this case, navigating to `/about` results in an incorrect component rendering or a blank page.  This is because the router might get confused as to which route to match.

## Solution

The solution involves removing the redundant route with the trailing slash.  React Router v6's route matching algorithm should handle this without any ambiguity.

## Setup

1. Clone the repository
2. `npm install`
3. `npm start`