# Auto-Food-Warehouse-System

## 📦 Project Description:
An intelligent warehouse system that relies on robots to automate the process of picking, transporting, and packaging food products. The system includes storage shelves, conveyor belts, and robots to handle product movement and packaging efficiently.

## ⚙️ System Components:
- Storage shelves stocked with food items.
- Robot 1 (Picker): Retrieves items from shelves and places them on conveyors.
- 3 Conveyor Belts: Move items to the packaging area.
- 3 Packaging Robots (Packer 1, 2, 3): Responsible for wrapping and placing items into the output zone.

## 🧠 System Algorithm:

```plaintext
Algorithm: AutomatedFoodWarehouse_MultiConveyor()

1. Start

2. Initialize:
   a. Storage shelves with food items
   b. Robot1 (Pick-and-Place) at the storage area
   c. Conveyor Belts: Conveyor1, Conveyor2, Conveyor3
   d. Packaging Robots: Packer1, Packer2, Packer3

3. While there are pending orders:

    a. Robot1 scans shelves for the requested product
    b. Picks the product from the shelf
    c. Selects an available conveyor (round-robin or least busy)
    d. Places the item onto the selected conveyor

    e. Conveyor transports the item to the packaging area

    f. The assigned Packaging Robot (based on conveyor):
        i. Detects the item on the conveyor
        ii. Picks up the item
        iii. Performs packaging
        iv. Places the packaged item in the output bin

4. Repeat the process for each new product

5. End
