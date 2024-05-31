# Developer Documentation

Welcome to the developer documentation for the BiologicalSimulation project! This document provides guidance for developers who want to contribute to or extend the project.

## Project Structure

The project is structured as follows:

```
BiologicalSimulation/
│
├── images_output/
│   ├── image_1.png
│   └── image_2.jpg
├── .gitignore
├── CODE_OF_CONDUCT.md
├── LICENSE
├── Project_Submission_explanation.md
├── README.md
├── biological_simulation_Observation.md
├── developer_docs.md
├── requirements.txt
└── simulation.py
```

- `images_output/`: Directory containing images generated as output by the simulation.
- `.gitignore`: File specifying patterns of files to be ignored by Git.
- `CODE_OF_CONDUCT.md`: Code of Conduct for contributors.
- `LICENSE`: File containing the project's license information.
- `Project_Submission_explanation.md`: Explanation of the project submission for documentation.
- `README.md`: Markdown file providing an overview of the project.
- `biological_simulation_Observation.md`: Document for recording observations and findings from the simulation.
- `developer_docs.md`: This document, providing guidance for developers.
- `requirements.txt`: File listing the project's dependencies.
- `simulation.py`: Main Python script containing the simulation logic.

## Contributing Guidelines

### Setting Up the Development Environment

1. Clone the repository:

    ```bash
    git clone https://github.com/yourusername/BiologicalSimulation.git
    cd BiologicalSimulation
    ```

2. Create a virtual environment:

    ```bash
    python -m venv venv
    ```

3. Activate the virtual environment:

    - **Windows**:

        ```bash
        .\venv\Scripts\activate
        ```

    - **macOS/Linux**:

        ```bash
        source venv/bin/activate
        ```

4. Install dependencies:

    ```bash
    pip install -r requirements.txt
    ```

### Running Tests

To run the unit tests, navigate to the project root directory and run:

```bash
python -m unittest discover -s tests -p '*_test.py'
```

### Coding Standards

- Follow PEP 8 style guidelines for Python code.
- Use meaningful variable and function names.
- Write docstrings for all classes and functions.
- Ensure backward compatibility when making changes.

### Branching Strategy

- Create a new branch for each feature or bug fix.
- Use descriptive branch names (e.g., `feature/new-entity`, `bugfix/collision-detection`).
- Make pull requests against the `main` branch.

### Code Reviews

- All changes must be reviewed before merging.
- Request reviews from at least one other team member.
- Address any feedback or comments before merging.

## Roadmap

### Planned Features

- Enhanced entity interactions.
- Advanced biological behaviors.
- Improved graphics and animations.

### Future Improvements

- Integration with external data sources.
- Real-time visualization of simulation data.
- Support for user-defined scenarios and parameters.

## Contact Information

If you have any questions or need assistance, feel free to reach out to the project maintainers:
https://www.instagram.com/rishit_katiyar/

Happy coding!
