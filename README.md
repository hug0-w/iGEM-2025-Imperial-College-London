# Growf - iGEM Imperial College London 2025

**🏆 Gold Medal Winner at iGEM 2025 🏆**

This repository contains the source code for the Imperial College London's 2025 iGEM team project, "Growf". You can find our full project wiki at [2025.igem.wiki/imperial/](https://2025.igem.wiki/imperial/).

## Abstract

The current model of meat production is environmentally unsustainable, driving deforestation, biodiversity loss, and global greenhouse gas emissions. Cultivated meat offers a promising alternative, yet remains hindered by high production costs, particularly the price of recombinant growth factors that constitute up to 70% of total media expenses. Our project, **Growf**, tackles this challenge by engineering a *Komagataella phaffii* chassis, **Mannoless**, designed to reduce exopolysaccharide (EPS) secretion and improve recombinant protein yield through targeted genetic modifications. In parallel, we developed **BioKernel**, an open-access, no-code Bayesian optimisation framework that accelerates experimental design and strain engineering, enabling researchers to identify optimal conditions with minimal experiments.

Guided by **Integrated Human Practices**, we engaged world-leading experts across academia and industry to explore unspoken pitfalls of scaling in yeast chassis. Our **Education** efforts addressed public skepticism toward cultivated meat and synthetic biology, recognising that innovation cannot scale without public trust and investor confidence.

We were on a mission to make all of our outputs, including genetic constructs, engineered strains, and software **fully open-access**, reaffirming our belief that science cannot scale without non-proprietary technology. We aimed to remove cost, accessibility, and licensing barriers in biomanufacturing, accelerating the scalability of cultivated meat and paving the way for a more sustainable, ethical, and open future for food.

## Our Solution

### MANNOLess

<span class="highlight-green">Mannoless</span> is our <em>K. phaffii</em> strain engineered to minimise <strong>exopolysaccharide (EPS) secretion</strong>, with the goal of freeing up more cellular energy for recombinant protein production and thereby increasing the yields of our proteins of interest. Specifically, we used a three-pronged strategy to target cell wall integrity and protein glycosylation pathways by modifying *Hoc1*, *Rho1* and *PMI* genes.

### BioKernel

**BioKernel** is our dry lab software platform designed to optimise experimental design and strain engineering in synthetic biology. It applies **Bayesian optimisation** to guide biological experiments toward optimal outcomes using minimal resources. The framework was developed to address a key challenge of biological research, the **high cost and limited throughput of experimental testing**, by allowing researchers to systematically explore complex parameter spaces arising in biological experimentation without requiring coding expertise.

BioKernel can be downloaded from: [https://gitlab.igem.org/2025/software-tools/imperial](https://gitlab.igem.org/2025/software-tools/imperial)

## Running the Website

This repository contains the Flask application that serves our iGEM wiki. To run it locally, follow these steps:

1.  **Clone the repository:**
    ```bash
    git clone <repository-url>
    cd <repository-directory>
    ```

2.  **Install dependencies:**
    Make sure you have Python and pip installed.
    ```bash
    pip install -r dependencies.txt
    ```

3.  **Run the application:**
    ```bash
    flask serve
    ```
    The website will be available at `http://localhost:8080`.

## Generating the Static Website

To generate a static version of the website (e.g., for deployment), run the following command:

```bash
flask freeze
```

This will create a `public` directory containing the static files.