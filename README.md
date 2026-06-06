# Python Word-in-File Check

A lightweight, memory-efficient file parsing utility designed to scan local text data, pinpoint exact keyword locations, and deliver precise line-by-line metrics.

## 🚀 Overview

This script solves a common data-parsing challenge: finding exactly where and how often a specific keyword appears within a file. Built with core Python principles, it provides a clean, interactive command-line interface to analyze text assets (like logs, scripts, or documentation) without any external dependencies.

## 🧠 Technical Highlights (Why it's built this way)

* **Memory-Optimized Stream Processing:** By utilizing `f1.txt` with sequential `readline()` iterations rather than loading the entire file into RAM, the script ensures a minimal memory footprint—making it scalable for larger log files.
* **Safe Resource Management:** Implements Pythonic context managers (`with open()`) to guarantee file streams are safely allocated and closed, preventing accidental memory leaks.
* **Granular Indexing:** Tracks and maps absolute line positions dynamically, making it a highly practical utility for debugging or pattern auditing.

## ✨ Key Features

* **Interactive User Input:** Dynamically queries the user for target keywords on execution.
* **Live Location Reporting:** Outputs the exact line index for every match in real-time.
* **Smart Summarization:** Evaluates data post-stream to give a final breakdown, gracefully handling instances where the target word does not exist.
