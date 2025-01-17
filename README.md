# Unhandled JSON Key Access in Dart Network Request

This repository demonstrates a common error in Dart applications that handle network requests and JSON parsing: accessing a key in a JSON response that might not exist.

The `bug.dart` file shows the problematic code.  The `bugSolution.dart` file provides a solution to safely access JSON data.

## Problem

The original code attempts to access `jsonData['key']` directly. If the JSON response doesn't contain a 'key', this will cause a runtime exception.

## Solution

The solution involves checking if the key exists before attempting to access it.  This prevents runtime errors and improves the robustness of the application.