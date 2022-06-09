
## VMDecomp

<br>

The **VMDecomp** R package is the *RcppArmadillo* implementation of the ["Variational Mode Decomposition" Matlab code](https://math.montana.edu/dzosso/code/) in R. More details on the functionality of VMDecomp can be found in the package *Documentation* and *Vignette*.

<br>

### Installation:

<br>

To install the package from CRAN use, 

```R
install.packages("VMDecomp")

```
<br>

and to download the latest version of the package from Github,

```R
remotes::install_github('mlampros/VMDecomp')

```

<br>

#### **Docker Image**

<br>

**Docker images** of the *VMDecomp* package are available to download from my [dockerhub](https://hub.docker.com/r/mlampros/vmdecomp) account. The images come with *Rstudio* and the *R-development* version (latest) installed. The whole process was tested on Ubuntu 18.04. To **pull** & **run** the image do the following,

<br>

```R

docker pull mlampros/vmdecomp:rstudiodev

docker run -d --name rstudio_dev -e USER=rstudio -e PASSWORD=give_here_your_password --rm -p 8787:8787 mlampros/vmdecomp:rstudiodev

```

<br>

The user can also **bind** a home directory / folder to the image to use its files by specifying the **-v** command,

<br>

```R

docker run -d --name rstudio_dev -e USER=rstudio -e PASSWORD=give_here_your_password --rm -p 8787:8787 -v /home/YOUR_DIR:/home/rstudio/YOUR_DIR mlampros/vmdecomp:rstudiodev


```

<br>

The **USER** defaults to *rstudio* but you have to give your **PASSWORD** of preference (see [www.rocker-project.org](https://www.rocker-project.org/) for more information).

<br>

Open your web-browser and depending where the docker image was *build / run* give, 

<br>

**1st. Option** on your personal computer,

<br>

```R
http://0.0.0.0:8787 

```

<br>

**2nd. Option** on a cloud instance, 

<br>

```R
http://Public DNS:8787

```

<br>

to access the Rstudio console in order to give your username and password.

<br>

### **Citation:**

If you use the **VMDecomp** R package in your paper or research please cite both **VMDecomp** and the **original articles / software** `https://CRAN.R-project.org/package=VMDecomp`:

<br>

```R
@Manual{,
  title = {{VMDecomp}: Variational Mode Decomposition using R},
  author = {Lampros Mouselimis},
  year = {2022},
  note = {R package version 1.0.0},
  url = {https://CRAN.R-project.org/package=VMDecomp},
}
```

<br>