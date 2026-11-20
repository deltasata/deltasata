## Satadru Bag

Data scientist in Munich with 12+ years of analysing large, noisy datasets and 7+ years of hands-on machine learning on images and time series. I lead the rare-event search in a 10,000-member international collaboration and build its ML and data systems: a real-time pipeline on Google Cloud (~10M events per night), transformer and ConvLSTM models that update their prediction with every new frame, and the image-processing chain that generates their training data. I also build agentic AI workflows for research that run large model searches under strict, pre-registered quality checks.

**Website:** [deltasata.github.io](https://deltasata.github.io): every project, results and CV.

**Personal projects**

| Project | What it does | Stack |
|---|---|---|
| [EO-Agent, conversational Earth-observation analyst](https://github.com/deltasata/satellite-change-agent) | LLM agent that answers "was this place flooded / built on?" from free satellite images, every number checked against deterministic code. Learned models replace rules only if they win on held-out flood events (pre-registered): water IoU 0.833 vs 0.690 (U-Net), flood questions answered correctly 0.889 vs 0.722; on par with the published state of the art. | PyTorch, TerraMind, Prithvi-EO, Claude Agent SDK, MCP, LangGraph, vLLM |

**Built for the rare-event search I lead**

| Project | What it does | Stack |
|---|---|---|
| [Real-time event pipeline](https://github.com/deltasata/LSST_alert_pipeline_LSN_search) | Stream and archive pipelines over six external data providers (REST APIs and Kafka, retries with back-off), a space-time SQL join on BigQuery and DuckDB, Parquet storage, a cost-guarded BigQuery layer and 500+ automated tests (ruff, mypy) in CI. | Python, REST APIs, Kafka (Avro), SQL (BigQuery, DuckDB), Google Cloud Storage, Parquet, pytest |
| [OASIS, transformers for asynchronous image streams](https://github.com/deltasata/OASIS--On-the-fly_ASynchronous_Image-Stream-classification) | Seven transformer architectures, chosen from 227 training runs across 19 architecture families, that score each new frame of an irregular multi-band image sequence: factorized vs joint space-time attention, windowed and pyramid variants and a Perceiver-style readout, with Time2Vec and causal masking; the best cut the recurrent baseline's loss by 30%; paper on arXiv (2610.17168). | PyTorch, Transformers, GPU |
| [Lean image-processing pipeline](https://github.com/deltasata/Stripped_down_LSST_Alert_Production_pipeline) | The production pipeline's image differencing (change detection), object detection and cross-frame tracking, run on small simulated cutouts to generate labelled training data at scale; every detection scored by two CNN quality models, checked against production. | Python, PyTorch, NumPy / SciPy, Apptainer |

**Rare-object search in survey images**

| Project | What it does | Stack |
|---|---|---|
| [Self-supervised ViTs for rare-object detection](https://github.com/deltasata/self-supervised-vit-lsst-lenses) | Finds rare objects (1 in thousands) in 5-band survey images. Automated model search (~60 architectures, ~300 GPU runs) with pre-registered comparisons; in-domain masked-autoencoder pretraining halved the loss; a ViT + ConvNeXtV2 ensemble reached AUC 0.9998 on a locked 30,000-object holdout, finding 90.6% at a 0.1% false-positive rate. | PyTorch, ViT, ConvNeXtV2, MAE, AMD MI300A |

**New statistical methods**

| Project | What it does | Stack |
|---|---|---|
| [Hidden echoes, a model-free statistic](https://github.com/deltasata/hidden-echo) | A random signal overlapping with its own delayed copy admits infinitely many exact splits; since 1996 the delay was thought impossible to find without a model of the signal. Every wrong split comes out rougher: that became a new statistic, with a proof of why it works. 92% precision under survey-grade noise, against 53% for autocorrelation. [ApJ 927, 191 (2022): method](https://arxiv.org/abs/2110.15315). [ApJ 950, 158 (2023): proof](https://arxiv.org/abs/2209.11078). | Time-series statistics, Blind validation |
| [Unresolved lensed supernovae, found from one blended light curve](https://github.com/deltasata/Unresolved_LSNeIa_in_LSST) | When the copies of a lensed supernova are too close to separate, a survey sees one blended light curve, and most lensed supernovae will look like that. Six years of work: recognising them from the curve's shape with methods that need hardly any template (under 5% false positives, under 0.5% delay bias), then a 1D CNN that flags them within about 20 days, and an LSTM (unpublished). Papers: [ApJ 910, 65 (2021)](https://arxiv.org/abs/2010.03774). [MNRAS 511 (2022)](https://arxiv.org/abs/2109.13282). [A&A 691, A100 (2024)](https://arxiv.org/abs/2404.15389). | Time-series statistics, Polynomial expansions, Microlensing models, 1D CNN, LSTM |

**Earlier work**

| Project | What it does | Stack |
|---|---|---|
| [ConvLSTM rare-event detector](https://github.com/deltasata/ConvLSTM-LSNe-Detection) | Spatio-temporal classifier for multi-band image time series that rescores every new frame: 70%+ recall at a 0.01% false-positive rate by the 9th image (128,000 training sequences). Papers: [A&A 707, A123 (2026), arXiv:2506.22076](https://arxiv.org/abs/2506.22076). [Part II, A&A in press, arXiv:2605.05318](https://arxiv.org/abs/2605.05318). | TensorFlow / Keras |
| [SURFGEN2 / Shapefinders](https://github.com/deltasata/Shapefinders) | 3D surface reconstruction and shape statistics on large 3D grids, used by several research groups. | C, MPI |

**Theory and mathematics (papers)**

| Project | What it does | Stack |
|---|---|---|
| Theory, dark energy and the expansion of the universe | Where the data work started: why the universe's expansion speeds up. Perturbation equations solved from the early universe to today, an analytic growth formula accurate to 0.1%, a stability analysis, a dark-energy model family free of fine-tuning, fits to survey data, and a diagnostic (2026) that avoids differentiating noisy data. 8 papers, 2014 – 2026. Papers: [JCAP 2014](https://arxiv.org/abs/1403.4243). [JCAP 2016](https://arxiv.org/abs/1603.01277). [JCAP 2018](https://arxiv.org/abs/1709.09193). [Phys. Rev. D 2018](https://arxiv.org/abs/1805.10405). [arXiv 2026](https://arxiv.org/abs/2605.27230). | Differential equations, Perturbation theory, Numerical methods, Bayesian inference |

**Stack:** Python · PyTorch · TensorFlow / Keras · SQL (BigQuery, DuckDB) · REST APIs · Google Cloud · AWS · Kafka · Docker / Apptainer · HPC (SLURM, CUDA / ROCm) · Testing (pytest, ruff, mypy)

**Also:** Generative models (diffusion, normalizing flows) · Simulation-based inference · Graph neural networks · LLM agents (MCP, LangGraph, Claude Agent SDK, OpenAI Agents SDK) · Bayesian inference

**Currently learning:** MLflow · Apache Spark · Google Earth Engine

PhD · 35+ research papers, 30+ peer-reviewed in Q1 journals (some in press) · [Website](https://deltasata.github.io) · [LinkedIn](https://www.linkedin.com/in/satadru-bag) · [Google Scholar](https://scholar.google.com/citations?user=tD5KssAAAAAJ&hl=en)

Open to Data Scientist / ML roles in Germany · EU Blue Card holder (Germany) · Available at short notice
