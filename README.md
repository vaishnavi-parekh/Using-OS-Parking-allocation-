# Using-OS-Parking-allocation-
An interactive web-based Parking Lot Allocation Simulator that compares First Fit, Best Fit, and Worst Fit algorithms using visualizations and space-utilization metrics. Built with HTML, CSS, and JavaScript.
Parking Lot Allocation Simulator
A browser-based simulator that demonstrates how First Fit, Best Fit, and Worst Fit allocation algorithms assign cars to parking slots of different sizes. The project connects a real-world parking scenario with the memory-allocation strategies studied in Operating Systems.
Features
- Compare First Fit, Best Fit, and Worst Fit in one run, or select a single algorithm.
- Enter custom parking-slot sizes and car sizes (in square feet).
- View a visual representation of occupied slots and unused space.
- See which cars could not be parked.
- Review a step-by-step allocation log.
- Compare results in tables and bar charts.
- Load sample data or generate random test data.
- Responsive layout for smaller screens.
- Light and dark appearance based on the device's color-scheme preference.
Technologies Used
- HTML5
- CSS3
- JavaScript (vanilla)
No framework, package installation, build step, or backend server is required.
Run Locally
1. Download or clone this repository.
2. Open index.html in a modern web browser.
3. Enter parking-slot sizes and car sizes, separated by commas.
4. Choose Compare all three, First Fit, Best Fit, or Worst Fit.
5. Click Park the cars to view the results.
Example input:
- Parking slot sizes: 100, 500, 200, 300, 600
- Car sizes: 212, 417, 112, 426
You can also use Load sample data or Random data.
How the Algorithms Work
- First Fit: Assigns each car to the first currently available slot that is large enough, scanning slots in their entered order.
- Best Fit: Assigns each car to the smallest currently available slot that can fit it.
- Worst Fit: Assigns each car to the largest currently available slot that can fit it.
Each slot can hold at most one car in this simulation. A slot is considered available only if no earlier car has been assigned to it.
Metrics Shown
- Cars parked: Number of cars successfully assigned to a slot.
- Not parked: Number of cars that could not fit into any remaining slot.
- Wasted space: Sum of the unused area in slots that were assigned to cars (slot size - car size).
- Space used: Total area of successfully parked cars divided by the total capacity of all slots, displayed as a percentage.
When comparing algorithms, the simulator highlights the result with the most cars parked, breaking ties by choosing the lower total wasted space. This is a comparison for the supplied input, not a guarantee that one algorithm is always best.
Input Rules and Limits
- Enter positive whole numbers for all slot and car sizes.
- Separate values with commas or spaces.
- Use no more than 12 slots and 12 cars at a time to keep the visual output readable.
- Sizes are illustrative and are treated as numeric units in square feet.

Deploy with GitHub Pages
1. Push the project files to a GitHub repository.
2. Open the repository's Settings.
3. Select Pages in the sidebar.
4. Under the build/deployment section, choose Deploy from a branch.
5. Select the main branch and the / (root) folder, then save.
6. Wait for GitHub Pages to publish the site. The live URL will appear in the Pages settings.
Future Improvements
- Add parking-slot labels and vehicle categories.
- Support multiple cars per slot when capacity permits.
- Add exportable reports for simulation results.
- Add automated tests for allocation scenarios.
- Separate HTML, CSS, and JavaScript into individual files.
License
No license has been specified yet. If you want others to reuse, modify, or distribute this project, consider adding an appropriate open-source license file, such as the MIT License, after deciding the terms you want to allow.
