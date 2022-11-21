<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/github_username/repo_name">
    <img src="images/GP2_logo.png" alt="Logo" width="300" height="70">
  </a>

<h3 align="center">Network generation and visualization pipeline</h3>

  <p align="center">
    One of the projects from the 2021 GP2/IPDGC Hackathon. The related manuscript can be found on [biorxiv](https://www.biorxiv.org/content/10.1101/2022.05.04.490670v1) 
    <br />
    Contributers: Dan Vitale, Jie Yuan, Thiago Peixoto Leal, Isabelle Foote, Gabriela Salazar
    <br />
  </p>
</div>



<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#quick-description">Quick Description</a></li>
        <li><a href="#background/motivation">Background/motivation</a></li>
        <li><a href="#workflow-summary">Workflow Summary</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project

![Project Screen Shot][project-screenshot]

### Quick Description

The goal for this project was to develop a pipeline that generates and visualizes gene regulatory networks.

### Background/motivation

Gene regulatory networks are important in understanding disease. This workflow serves as an example for how to build leiden networks with eQTL and genetic data with the leidenalg python package.     

### Workflow Summary

1. Pull genes - this includes querying QTLs from open targets API in brain tissues to connect SNPs to genes.
2. Extract from AMP data.
3. Build correlation / graph space in cases.
4. Leiden to build communties.
5. Vizualize.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- GETTING STARTED -->
## Getting Started

### Prerequisites

* Check hackathon_networks.ipynb for the list of required Python packages 

### Installation

1. Clone the repo
   ```sh
   git clone https://github.com/ipdgc/GP2-network-generation.git
   ```

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- USAGE EXAMPLES -->
## Usage

This notebook was built with AMP-PD and eQTL data from eQTLGen and mined from opentargets, but by changing the file paths you can use any data of choice.


### 1. Use the hackathon_networks.ipynb notebook 

This will walk you through set up, generation of the network, and visualization of the network.


_For more examples, please refer to leidenalg [documentation](https://readthedocs.org/projects/leidenalg/downloads/pdf/latest/)_

<p align="right">(<a href="#readme-top">back to top</a>)</p>


<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

* [OpenTargets](https://genetics.opentargets.org/)
* [eQTLGen](https://www.eqtlgen.org/)

<p align="right">(<a href="#readme-top">back to top</a>)</p>


<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[project-screenshot]: images/project_screenshot.png

