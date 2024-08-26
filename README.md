
# Sorting Algorithm Visualizer

This Python project provides an interactive way to visualize and understand the inner workings of various sorting algorithms using the Tkinter library. It's an educational tool designed to help users grasp how different algorithms handle data and progress towards sorting.

## Features

- **Interactive Visualization:** Watch as the selected sorting algorithm processes data step-by-step, with each operation clearly illustrated by color changes.
- **Multiple Sorting Algorithms:** Currently, the visualizer supports:
  - **Bubble Sort:** A simple comparison-based algorithm where each pair of adjacent elements is compared and swapped if they are in the wrong order.
  - **Selection Sort:** An in-place comparison sort where the list is divided into a sorted and an unsorted region, and the smallest element from the unsorted region is moved to the end of the sorted region.
  - **Insertion Sort:** An algorithm that builds the final sorted array one item at a time, by repeatedly picking the next item and inserting it into its correct position within the sorted section.
- **Customizable Settings:**
  - **Array Size:** Adjust the size of the data set to see how the algorithms perform with different input sizes.
  - **Visualization Speed:** Modify the speed at which the algorithm progresses, allowing you to slow down or speed up the sorting process.
- **Real-Time Feedback:** The visualizer provides immediate feedback on the sorting process, making it easier to understand how the algorithm works.

## Program Overview

The sorting algorithm visualizer is built with a strong focus on educational value. Each algorithm is implemented as a function that interacts with a drawing function to update the visual representation of the data array.

### Code Structure

- **Sorting Algorithms:** The main sorting algorithms are defined in separate functions within the script. These functions include logic for sorting and update the display at each significant step using the drawData function.

- **GUI Setup:** Tkinter is used to create the graphical interface, including sliders for adjusting array size and speed, dropdowns for selecting algorithms, and buttons to control the visualization.The interface is designed to be intuitive, making it easy for users of all levels to start visualizing sorting algorithms with minimal setup.

- **Visualization Logic:** The drawData function is central to the visualizer, controlling how the data array is rendered on the screen. The function uses colors to represent different states of the data (e.g., unsorted, currently being compared, sorted).

### Key Functions

- **drawData(data, colorArray)**: This function is responsible for updating the canvas with the current state of the array. It draws rectangles of varying heights, representing the array elements, and uses colors to indicate their current state.

- **startAlgorithm()**: This function is triggered when the user starts the visualization. It captures the selected algorithm and settings, then calls the corresponding sorting function.

- **generateData()**: This function creates a random list of integers based on the user's input for array size. The generated list is what gets sorted by the algorithms.


    

### User Interface

- **Algorithm Dropdown:** Select the algorithm you want to visualize from the dropdown menu.
- **Array Size Slider:** Use this slider to adjust the number of elements in the array. A larger array provides a more detailed view of the algorithm's performance.
- **Speed Slider:** Control the speed of the visualization. Slower speeds allow for a detailed examination of each step, while faster speeds show the overall process quickly.
- **Start Button:** Once you've configured the settings, click 'Start' to begin the visualization.
- **Time Complexity Display:** The program shows the time complexity of the selected sorting algorithm, providing theoretical insights alongside the practical visualization.

