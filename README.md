# Latex CV

Inspired from [liantze](https://github.com/liantze/AltaCV).

## Steps to compile

> Install Dokcer, VScode and [LaTeX-Workshop VSCode extension](https://marketplace.visualstudio.com/items?itemName=James-Yu.latex-workshop).

1. Pull tianon/latex image:

    ```shell
    docker pull tianon/latex
    ```

2. Open settings.json from vscode's command palette [CTRL+SHIFT+P]

    ![command palette](https://i.postimg.cc/xdxnHkSn/1-Xzewrv5f2-FBAfv2t1-Dko-Tw.png)

3. Add the following snippet

    ```json
    {
        // ... YOUR OTHER SETTINGS ...
        // latex
        "latex-workshop.docker.enabled": true,
        "latex-workshop.latex.outDir": "./out",
        "latex-workshop.synctex.afterBuild.enabled": true,
        "latex-workshop.view.pdf.viewer": "tab",
        "latex-workshop.docker.image.latex": "tianon/latex",
        // End
      }
    ```

4. Use the LaTeX-Workshop VSCode extension to compile and view the output file.

## How it works?

  ![diagram](https://i.postimg.cc/GpRT65v3/shapes.png)
  