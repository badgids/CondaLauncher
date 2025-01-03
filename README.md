# CondaLauncher

![CondaLauncher Main Screen](https://github.com/ThisModernDay/CondaLauncher/blob/main/data/main.png?raw=true)

CondaLauncher is a Python application that allows you to manage and launch applications in different Conda environments.

![CondaLauncher Processes Modal](https://github.com/ThisModernDay/CondaLauncher/blob/main/data/running.png?raw=true)

## Platform Support

- Currently, the application only supports Windows. Mac support is coming soon.

## Features

- List and manage applications with their associated Conda environments
- Launch applications in their respective Conda environments
- Monitor running processes and view their output
- Manage application configurations through a YAML file
- Edit the applications YAML file directly within the app

![CondaLauncher Manage Applications](https://github.com/ThisModernDay/CondaLauncher/blob/main/data/manage.png?raw=true)

## Prerequisites

- [Miniconda](https://docs.conda.io/en/latest/miniconda.html) or [Anaconda](https://www.anaconda.com/products/distribution) installed on your system
- Python 3.10

## Installation

1. Clone the repository:
   ```
   git clone https://github.com/thismodernday/CondaLauncher.git
   cd CondaLauncher
   ```

2. Create a new Conda environment:
   ```
   conda create -n conda-launcher python=3.10
   ```

3. Activate the environment:
   ```
   conda activate conda-launcher
   ```

4. Install the required packages:
   ```
   pip install -r requirements.txt
   ```

5. Rename the example configuration file:
   ```
   mv example_applications.yaml applications.yaml
   ```

## Configuration

1. Open the `applications.yaml` file in the project root directory.
2. Edit the file to add your applications and their corresponding Conda environments. You can do this directly in the CondaLauncher application by clicking the "Manage Applications" button, or manually edit the file.
3. The format for each application is as follows:
   ```yaml
   applications:
     - name: "App Name"
       conda_env: "environment_name"
       path: "/path/to/your/app.py"
       description: "Brief description of the app"
   ```

## Usage

1. Ensure you're in the CondaLauncher directory and your conda-launcher environment is activated.

2. Run the application:
   ```
   python Launcher.py
   ```

3. Use the interface to select, launch, and manage your applications:
   - Select an application from the list to view its details
   - Click "Launch" to start the selected application
   - Click "Manage Applications" to edit the applications.yaml file within the app
   - Use "Ctrl+O" to open the Processes Modal and view running applications

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
