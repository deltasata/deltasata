## Satadru Bag

Data scientist in Munich with 12 years of analysing large, noisy datasets and 7+ years of hands-on machine learning on images and time series. I lead the rare-event search in a 10,000-member international collaboration and build its ML and data systems: a real-time pipeline on Google Cloud (~10M events per night), transformer and ConvLSTM models that update their prediction with every new frame, and the image-processing chain that generates their training data.

**Now building: EO-Agent.** Conversational agent that answers "did this change happen here?" (flood, construction, vegetation loss) from Sentinel-2 images, with grounding checks in code on every number. Stack: Claude Agent SDK, MCP, LangGraph, vLLM (Qwen3-8B), Sentinel-2, PyTorch. Repo coming soon.

**Built for the rare-event search I lead**

| Project | What it does | Stack |
|---|---|---|
| [Real-time event pipeline](https://github.com/deltasata/LSST_alert_pipeline_LSN_search) | Stream and archive pipelines that collect, cross-match and store events from six external data providers (APIs), with a cost-guarded BigQuery layer and offline tests. | Python, Kafka, BigQuery (GCP), Parquet, pytest |
| [OASIS, transformers for asynchronous image streams](https://github.com/deltasata/OASIS--On-the-fly_ASynchronous_Image-Stream-classification) | Seven attention architectures that score each new frame of an irregular multi-band image sequence; paper on arXiv (2610.17168). | PyTorch, GPU |
| [Lean image-processing pipeline](https://github.com/deltasata/Stripped_down_LSST_Alert_Production_pipeline) | The production change-detection, object-detection and tracking steps, cut down to generate labelled training data at scale. | Python, Apptainer, CNN scoring |

**Earlier work**

| Project | What it does | Stack |
|---|---|---|
| [ConvLSTM rare-event detector](https://github.com/deltasata/ConvLSTM-LSNe-Detection) | Spatio-temporal classifier for multi-band image time series, trained on 128,000 sequences; published in A&A (2026), follow-up on arXiv (2605.05318). | TensorFlow / Keras |
| [SURFGEN2 / Shapefinders](https://github.com/deltasata/Shapefinders) | 3D surface reconstruction and shape statistics on large 3D grids, used by several research groups. | C, OpenMP |
| [Overlapping-signal 1D CNN](https://github.com/deltasata/Unresolved_LSNeIa_in_LSST) | Simulated overlapping-signal time series and a 1D CNN that detects them; data on Zenodo. | Python, TensorFlow, emcee |

**Stack:** Python · PyTorch · TensorFlow / Keras · SQL (BigQuery) · Google Cloud · AWS · Kafka · Docker / Apptainer · HPC (SLURM, GPUs)

**Also:** Generative models (diffusion, normalizing flows) · Simulation-based inference · Graph neural networks · LLM agents (MCP, LangGraph) · Bayesian inference

**Currently learning:** MLflow · Apache Spark · Google Earth Engine & Sentinel-2

PhD · 35+ research papers, 30+ peer-reviewed in Q1 journals (some in press); 570+ citations, h-index 14 · [LinkedIn](https://www.linkedin.com/in/satadru-bag) · [Google Scholar](https://scholar.google.com/citations?user=tD5KssAAAAAJ&hl=en)

Open to Data Scientist / ML roles in Germany · EU Blue Card holder (Germany) · Available at short notice
