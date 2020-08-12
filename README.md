# hello world example

Hello World application to get started building interactive dashboards with voila.

This example uses a conda `environment.yml` file to list the dependencies.

For an example using `requirements.txt`, you can check [render-stl](https://github.com/voila-gallery/render-stl) or [gaussian-density](https://github.com/voila-gallery/gaussian-density).


## Local Setup


To test the application locally:

```bash
conda env create
conda activate voila-gallery-hello-world-example

voila app.ipynb
```

This will open a new browser tab at [http://localhost:8866](http://localhost:8866) serving the dashboard.


## Testing on Binder


An environment file is all you need to make the dashboard work with Binder:

1. Go to [mybinder.org](https://mybinder.org)
2. Put the URL of the repository
3. Then select `Url` instead of `File`
4. Put the following URL in the `URL to open (optional)` field: `/voila/render/app.ipynb`

The repository is now ready to be used on [Binder](https://mybinder.org)!

More details about Binder can be found [in the documentation](https://mybinder.readthedocs.io/en/latest/introduction.html#preparing-a-repository-for-binder).

## The Binder process

1. How it works

Enter your repository information
Provide in the above form a URL or a GitHub repository that contains Jupyter notebooks, as well as a branch, tag, or commit hash. Launch will build your Binder repository. If you specify a path to a notebook file, the notebook will be opened in your browser after building.

2. We build a Docker image of your repository
Binder will search for a dependency file, such as requirements.txt or environment.yml, in the repository's root directory (more details on more complex dependencies in documentation). The dependency files will be used to build a Docker image. If an image has already been built for the given repository, it will not be rebuilt. If a new commit has been made, the image will automatically be rebuilt.

3. Interact with your notebooks in a live environment!
A JupyterHub server will host your repository's contents. We offer you a reusable link and badge to your live repository that you can easily share with others.
