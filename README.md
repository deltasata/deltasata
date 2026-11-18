## Satadru Bag

Data scientist in Munich. I build machine-learning systems that find rare events in large streams of images and time series: real-time data pipelines on Google Cloud, and deep-learning models (transformers, ConvLSTMs, CNN ensembles) that update their prediction with every new observation.

**What I have built**

- A real-time pipeline that ingests ~10M events (~1 TB) per night from six external APIs and Kafka streams, with a cost-guarded BigQuery layer → [`LSST_alert_pipeline_LSN_search`](https://github.com/deltasata/LSST_alert_pipeline_LSN_search)
- OASIS: seven transformer architectures for irregular multi-band image streams; factorized attention cut the loss by 30% against a ConvLSTM baseline → [`OASIS`](https://github.com/deltasata/OASIS--On-the-fly_ASynchronous_Image-Stream-classification)
- A ConvLSTM model that flags rare events in image time series at a 0.01% false-positive rate → [`ConvLSTM-LSNe-Detection`](https://github.com/deltasata/ConvLSTM-LSNe-Detection)
- SURFGEN2, a C/OpenMP package for 3D surface modelling used by several research groups → [`Shapefinders`](https://github.com/deltasata/Shapefinders)

**Now building: EO-Agent.** Conversational agent that answers "did this change happen here?" (flood, construction, vegetation loss) from Sentinel-2 images, with grounding checks in code on every number. Stack: Claude Agent SDK, MCP, LangGraph, vLLM (Qwen3-8B), Sentinel-2, PyTorch. Repo coming soon.

**Stack:** Python · PyTorch · TensorFlow / Keras · SQL (BigQuery) · Google Cloud · Kafka · Docker / Apptainer · HPC (SLURM, GPUs)

**Currently learning:** MLflow · Apache Spark · Google Earth Engine & Sentinel-2

PhD · 35+ research papers, 28 peer-reviewed in Q1 journals; 570+ citations, h-index 14 · [LinkedIn](https://www.linkedin.com/in/satadru-bag) · [Google Scholar](https://scholar.google.com/citations?user=tD5KssAAAAAJ&hl=en)
