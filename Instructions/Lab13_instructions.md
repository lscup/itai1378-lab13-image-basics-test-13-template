# Image Basics Test 13 Assignment

## Overview
In this assignment, you will enhance your Jupyter Notebook to complete the Image Basics test 13 by implementing specific features. Your goal is to modify the existing starter code to match the solution code provided.

## Learning Objectives
- Understand how to manipulate images using provided functions.
- Implement code to achieve desired image transformations.
- Validate your implementation against test cases.

## Your Coding Environment
You will work within a Jupyter Notebook environment. The interface has two primary tabs: the code editing tab where you'll write your code, and the output tab where you can see the results of running your code. To execute your code, use the **Run button**. After editing and running, you can save your progress by clicking the **Commit button**. You'll receive feedback from the autograder which will indicate success with a ✅ or failure with a ❌ based on the tests.

## Workflow
1. Edit your code in the Jupyter Notebook.
2. Click the **Run button** to execute your code.
3. Use the **Commit button** to save your changes.
4. Check the autograder feedback to see if your implementation passes the tests ([32m✅[39m or [31m❌[39m).

## Implementation Instructions
1. **Image Import**: Modify the code to include an image import statement. Add the following line:
   ```python
   from PIL import Image
   ```
   This imports the necessary library for image manipulation.

2. **Loading the Image**: Implement the image loading functionality. After any necessary definitions, add:
   ```python
   image = Image.open('path/to/image.jpg')
   ```
   Ensure you replace `'path/to/image.jpg'` with the correct path to your image file.

3. **Image Manipulation**: Add a new function for manipulating the image. Create a function called `process_image()` and include the following code inside it:
   ```python
   def process_image(image):
       # Example transformation
       image = image.convert('L')  # Convert to grayscale
       return image
   ```

4. **Display the Image**: After processing, ensure to display the image. Add:
   ```python
   processed_image = process_image(image)
   processed_image.show()
   ```

5. **Implement Tests**: Finally, ensure that the provided tests are included in your notebook. Make sure the tests validate the output of your image processing functions correctly.

## Example Usage
Make sure to test your implementation by calling `process_image(image)` after loading the image. The image should be displayed in its processed form.

## Hints & Tips
- Ensure the path to your image file is correct to avoid file not found errors.
- If the image does not display, double-check that your `process_image()` function is returning the modified image correctly.
- Test each part of your implementation step by step to identify where issues may arise.