---
layout: post
title: "How To Create TableView"
date: 2022-12-28 08:16:04 +0700
categories: jekyll update
---

1. Open Main.storyboard: In the project navigator, double-click on the Main.storyboard file to open the Interface Builder.

2. Add a UITableView: From the Object Library (bottom-right panel), search for "Table View" and drag and drop it onto the canvas of the view controller.

3. Configure the UITableView: Select the table view on the canvas, and in the Attributes Inspector (right-side panel), customize the appearance and behavior of the table view. Set the number of prototype cells, adjust row height, and enable any desired features such as section headers or footers.

4. Create a UITableViewCell prototype: Select the table view on the canvas, and in the Attributes Inspector, set the "Prototype Cells" value to the desired number of cells. Customize each prototype cell by dragging UI elements (labels, images, etc.) onto the cell.

5. Configure UITableView data source and delegate: Open the Assistant Editor by clicking the icon in the top-right corner of Xcode's editor. Make sure the storyboard is visible in the left pane, and the view controller's code is visible in the right pane. Ctrl-drag from the table view to the view controller's code to create an outlet for the table view. Also, make the view controller conform to the `UITableViewDataSource` and UITableViewDelegate protocols.

6. Implement `UITableViewDataSource` methods: In the view controller's code, implement the required methods of the `UITableViewDataSource` protocol to provide data to the table view. These methods include `numberOfSections`(in:), `tableView`(_:numberOfRowsInSection:), and `tableView`(_:cellForRowAt:). Return the appropriate values and configure the cells with the desired data.

7. Implement `UITableViewDelegate` methods (optional): If you need to handle user interactions with the table view, implement the relevant methods of the `UITableViewDelegate` protocol. These methods include `tableView`(_:didSelectRowAt:), `tableView`(_:heightForRowAt:), and `tableView`(_:viewForHeaderInSection:), among others.

8. Build and run the project: Press Cmd+R or click the "Run" button in Xcode's toolbar to build and run the project in the iOS Simulator or a connected device. You should see your table view with the configured cells.
