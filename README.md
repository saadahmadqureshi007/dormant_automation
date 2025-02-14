
This script processes device and tenant data files, generating a `master.xlsx` file in the `output` folder. The input files are then moved to the `executed` folder to prevent re-processing in the future.

## Prerequisites

- **Node.js**: Make sure you have the latest version of Node.js installed. You can download it from [Node.js official website](https://nodejs.org/).

## Setup Instructions

Follow these steps to set up and run the script:

1. **Clone the Repository**

   Clone the repository using the following command:
   ```bash
   git clone <repository-url>
   ```

2. **Navigate to the Project Directory**

   ```bash
   cd <project-directory>
   ```

3. **Pull the Latest Code from the Main Branch**

   Make sure you're working with the latest code by pulling from the main branch:
   ```bash
   git pull origin main
   ```

4. **Delete .gitkeep Files**

   Delete any `.gitkeep` files inside the `input/devices` and `input/tenants` folders:
   ```bash
   rm input/devices/.gitkeep
   rm input/tenants/.gitkeep
   ```

5. **Install Dependencies**

   Install the required Node.js packages:
   ```bash
   npm install
   ```

6. **Place Input Files**

   - Place the devices file in the `input/devices` folder.
   - Place the tenants file in the `input/tenants` folder.

7. **Run the Script**

   Execute the script using the following command:
   ```bash
   node index.js
   ```

8. **Check the Output**

   After running the script:
   - The `master.xlsx` file will be generated in the `output` folder.
   - Your input files will be moved to the `executed` folder to avoid re-processing them in the future.

## Folder Structure

```
project-directory/
├── input/
│   ├── devices/
│   │   └── <devices-file>
│   ├── tenants/
│   │   └── <tenants-file>
├── executed/
├── output/
│   └── master.xlsx
├── index.js
└── README.md
```

## Troubleshooting

- **Ensure that the input files are correctly placed in the `input/devices` and `input/tenants` folders before running the script.**
- **Make sure all dependencies are installed by running `npm install` if you encounter any missing module errors.**

## License

This project is licensed under the MIT License.
```

Replace `<repository-url>` and `<project-directory>` with the actual values as needed. Let me know if you need further changes!
