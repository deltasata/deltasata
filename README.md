## Satadru Bag

Data scientist in Munich with 12 years of analysing large, noisy datasets and 7+ years of hands-on machine learning on images and time series. I lead the rare-event search in a 10,000-member international collaboration and build its ML and data systems: a real-time pipeline on Google Cloud (~10M events per night), transformer and ConvLSTM models that update their prediction with every new frame, and the image-processing chain that generates their training data.

**Personal projects**

| Project | What it does | Stack |
|---|---|---|
| [EO-Agent, conversational Earth-observation analyst](https://github.com/deltasata/satellite-change-agent) | LLM agent that answers "was this place flooded / built on?" from free satellite images, every number checked against deterministic code. Learned models replace rules only if they win on held-out flood events (pre-registered): water IoU 0.833 vs 0.690 (U-Net), flood questions answered correctly 0.889 vs 0.722; on par with the published state of the art. | PyTorch, TerraMind, Prithvi-EO, MCP, LangGraph, vLLM |

**Coming soon: Self-supervised ViTs for rare-object detection.** Finds strongly lensed quasars (about 1 in thousands of objects) in simulated 5-band survey images. Stack: PyTorch, ViT, ConvNeXtV2, MAE, AMD MI300A.

**Built for the rare-event search I lead**

| Project | What it does | Stack |
|---|---|---|
| [Real-time event pipeline](https://github.com/deltasata/LSST_alert_pipeline_LSN_search) | Stream and archive pipelines that pull events from six external data providers through REST APIs and Kafka (retries with back-off), cross-match them with a space-time SQL join that runs on both BigQuery and DuckDB, and store them as Parquet; cost-guarded BigQuery layer, typed config, CLI and 500+ automated tests (ruff, mypy) run in CI. | Python, REST APIs, Kafka (Avro), SQL (BigQuery, DuckDB), Google Cloud Storage, Parquet, pytest |
| [OASIS, transformers for asynchronous image streams](https://github.com/deltasata/OASIS--On-the-fly_ASynchronous_Image-Stream-classification) | Seven transformer architectures that score each new frame of an irregular multi-band image sequence: factorized vs joint space-time attention, windowed and pyramid variants and a Perceiver-style latent readout, with Time2Vec time embeddings and causal masking; evaluated at the real 8.5% positive rate; paper on arXiv (2610.17168). | PyTorch, transformers, GPU |
| [Lean image-processing pipeline](https://github.com/deltasata/Stripped_down_LSST_Alert_Production_pipeline) | The production pipeline's PSF-matched image differencing (change detection), object detection and measurement, and cross-frame association (tracking), run on small simulated cutouts to generate labelled training data at scale; every detection scored by two CNN quality models, with documented checks against production behaviour. | Python, PyTorch, NumPy / SciPy, Apptainer |

**Earlier work**

| Project | What it does | Stack |
|---|---|---|
| [ConvLSTM rare-event detector](https://github.com/deltasata/ConvLSTM-LSNe-Detection) | Spatio-temporal classifier for multi-band image time series, trained on 128,000 sequences; published in A&A (2026), follow-up on arXiv (2605.05318). | TensorFlow / Keras |
| [SURFGEN2 / Shapefinders](https://github.com/deltasata/Shapefinders) | 3D surface reconstruction and shape statistics on large 3D grids, used by several research groups. | C, MPI |
| [Overlapping-signal 1D CNN](https://github.com/deltasata/Unresolved_LSNeIa_in_LSST) | Simulated overlapping-signal time series and a 1D CNN that detects them; data on Zenodo. | Python, TensorFlow, emcee |

**Stack:** Python · PyTorch · TensorFlow / Keras · SQL (BigQuery, DuckDB) · REST APIs · Google Cloud · AWS · Kafka · Docker / Apptainer · HPC (SLURM, GPUs) · Testing (pytest, ruff, mypy)

**Also:** Generative models (diffusion, normalizing flows) · Simulation-based inference · Graph neural networks · LLM agents (MCP, LangGraph) · Bayesian inference

**Currently learning:** MLflow · Apache Spark · Google Earth Engine

PhD · 35+ research papers, 30+ peer-reviewed in Q1 journals (some in press); 570+ citations, h-index 14 · [LinkedIn](https://www.linkedin.com/in/satadru-bag) · [Google Scholar](https://scholar.google.com/citations?user=tD5KssAAAAAJ&hl=en)

Open to Data Scientist / ML roles in Germany · EU Blue Card holder (Germany) · Available at short notice
