---
layout: page
permalink: /repositories/
title: Repositories
description: Open computational databases supporting our research.
nav: true
nav_order: 5
_styles: |
  .research-data {
    margin: 2rem 0;
  }
  .research-data + .research-data {
    padding-top: 1.5rem;
    border-top: 1px solid var(--section-border, #cddabc);
  }
  .research-data .data-details {
    font-size: 0.95rem;
  }
  .research-data .data-actions {
    margin: 1rem 0;
  }
  .research-data .data-button {
    display: inline-block;
    max-width: 100%;
    padding: 0.6rem 1rem;
    border: 1px solid var(--section-border, #cddabc);
    border-radius: 5px;
    background: var(--section-bg, #e3eadb);
    color: var(--section-text, #475d36) !important;
    font-weight: 600;
    text-decoration: none;
    line-height: 1.5;
  }
  .research-data .data-button:hover {
    text-decoration: underline;
  }
  .research-data .data-button:focus-visible {
    outline: 3px solid var(--section-text, #475d36);
    outline-offset: 3px;
  }
  .research-data .data-doi {
    font-size: 0.9rem;
    overflow-wrap: anywhere;
  }
  .research-data .data-doi a {
    color: var(--global-text-color);
    text-decoration: underline;
  }
---

Explore the data behind our computational studies. Both databases are openly available on Zenodo, where you can browse the files, download the calculations, and find citation information.

<section class="research-data" aria-labelledby="benzene-database">
  <h2 id="benzene-database">Benzene and C₆ ring formation</h2>

  <p><strong>Comprehensive Computational Automated Search of Barrierless Reactions Leading to the Formation of Benzene and Other C6-Membered Rings</strong></p>

  <p>This database collects computational results from an automated search for barrierless pathways to benzene and other six-carbon rings. The data are organised by molecular fragment and include PM7 calculations and higher-level M08HX/6-31+G(d,p) results.</p>

  <p class="data-details"><strong>2024</strong> · Open data · CC BY 4.0</p>

  <p class="data-actions"><a class="data-button" href="https://zenodo.org/records/11175641" aria-label="Open the benzene and C6 ring formation database on Zenodo">Open database on Zenodo →</a></p>

  <p class="data-doi">DOI: <a href="https://doi.org/10.5281/zenodo.10776529">10.5281/zenodo.10776529</a></p>
</section>

<section class="research-data" aria-labelledby="damn-database">
  <h2 id="damn-database">Diaminomaleonitrile fragmentation</h2>

  <p><strong>Fragmentation Pathways of Diaminomaleonitrile: Automated Discovery and High-Level Energetics under Laser-Driven Conditions</strong></p>

  <p>This database provides the computational data for our study of diaminomaleonitrile (DAMN) fragmentation under laser-driven conditions. It includes PM7 and M08HX/6-31+G(d,p) calculations, together with DLPNO-CCSD(T)/cc-pVTZ single-point energies used to refine the energetics of DFT-optimised stationary points.</p>

  <p class="data-details"><strong>2026</strong> · Open data · CC BY 4.0</p>

  <p class="data-actions"><a class="data-button" href="https://zenodo.org/records/18213685" aria-label="Open the diaminomaleonitrile fragmentation database on Zenodo">Open database on Zenodo →</a></p>

  <p class="data-doi">DOI: <a href="https://doi.org/10.5281/zenodo.18213684">10.5281/zenodo.18213684</a></p>
</section>
