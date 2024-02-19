# Web Navigator

**Description:**
The Web Navigator project simulates the navigational operations of a web browser, including opening a new web page, navigating back a page, and going forward a page. The implementation utilizes the Stack class to maintain the history of visited pages with separate stacks for backPages and nextPages.

## Requirements

- **Node.js:**
  - Ensure that Node.js is installed on your system. You can download it from [nodejs.org](https://nodejs.org/).

- **prompt-sync:**
  - The program requires the 'prompt-sync' module. To install it, run the following command in your project directory:
    ```bash
    npm install prompt-sync
    ```

## Functionality

1. **Opening a New Web Page:**
   - When opening a new page, the previous page is pushed onto the backPages stack.
   - Any content in the nextPages stack is cleared.

2. **Navigating Back a Page:**
   - Revisiting an old page pushes the current page onto the nextPages stack.
   - The back operation is enabled or disabled based on the state of the backPages stack.

3. **Navigating Forward a Page:**
   - Revisiting a back page pushes the current page onto the nextPages stack.
   - The forward operation is enabled or disabled based on the state of the nextPages stack.

## User Input

User input is required for the following actions:

- Enter a new page to be visited.
- Navigate backward or forward a page.
- Quit the program.

The options for navigating forward or backward are conditional based on user input and the state of the stacks.

## Display

At every operation, excluding quitting, information about the current page and the top element of both the backPages and nextPages stacks is displayed.
