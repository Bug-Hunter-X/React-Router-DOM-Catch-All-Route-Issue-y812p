# React Router DOM Catch-All Route Issue

This repository demonstrates an uncommon bug in React Router DOM v6 related to catch-all routes (`/*`). The catch-all route is unexpectedly triggered even when a valid route exists, causing unexpected behavior.

## Bug Description

The issue arises when a catch-all route (`/*`) is defined alongside other routes.  Despite having routes such as `/` and `/about`, the catch-all route is always selected, overriding the intended navigation.

## Solution

The solution involves carefully ordering routes.  Catch-all routes should always be placed last in the Routes component to ensure they are only triggered when no other route matches.

## Setup

Clone the repo and run `npm install` to install the dependencies.

Start the development server using `npm start`.