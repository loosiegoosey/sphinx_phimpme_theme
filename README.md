
Overview
The **Sphinx FOSSASIA Theme** is a custom Sphinx theme specifically designed for FOSSASIA's projects. It provides an aesthetically pleasing and functional theme for Sphinx-generated documentation.

##
Features
- Custom HTML theme tailored for FOSSASIA's projects.
- Easy integration with Sphinx.
- Theme installation via standard Python packaging tools.

##
Installation Instructions

### Prerequisites
- Python 3.x installed on your system.
- `pip` (Python package installer).

### Steps
1. Clone the repository:
    ```sh
    git clone https://github.com/fossasia/sphinx_phimpme_theme.git
    ```

2. Navigate to the project directory:
    ```sh
    cd sphinx_phimpme_theme
    ```

3. Install the theme using `setup.py`:
    ```sh
    python setup.py install
    ```

##
Usage Examples

### Adding the Theme to a Sphinx Project

1. Edit your `conf.py` file in your Sphinx project directory to include the FOSSASIA theme:

    ```python
    import sphinx_fossasia_theme
    
    html_theme = 'sphinx_fossasia_theme'
    html_theme_path = [sphinx_fossasia_theme.get_html_theme_path()]
    ```

2. Build your Sphinx documentation:
    ```sh
    make html
    ```

Your Sphinx documentation will now use the FOSSASIA theme.

##
Code Summary

### File: `setup.py`
This file is responsible for setting up the theme package. It includes metadata such as the package name, version, author information, and other details required for distributing the theme.

### File: `sphinx_fossasia_theme/__init__.py`
This file contains functions to set up the theme with Sphinx:
- `setup(app)`: Adds the theme to the Sphinx app.
- `get_html_theme_path()`: Returns the absolute path to the theme directory.

##
Contributing Guidelines

We welcome contributions from the community to improve this project. To contribute:

1. Fork the repository.
2. Create a new branch with a descriptive name:
    ```sh
    git checkout -b feature/your-feature-name
    ```
3. Make your changes and commit them:
    ```sh
    git commit -am 'Add some feature'
    ```
4. Push to your branch:
    ```sh
    git push origin feature/your-feature-name
    ```
5. Create a pull request.

Please ensure your code follows the project's coding standards and includes appropriate tests if necessary.

##
License
This project is licensed under the GNU General Public License. See the [LICENSE](https://github.com/fossasia/sphinx_phimpme_theme/blob/main/LICENSE) file for more details.