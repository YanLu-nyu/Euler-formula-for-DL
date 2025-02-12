# Rencet Research of Big Companies (2022-)
## OpenAI
0. [(April, 2023) Consistency Models](https://arxiv.org/abs/2303.01469)
1. [(Mar, 2023) GPT-4](https://openai.com/research/gpt-4)
2. [(Oct, 2022) Scaling laws for reward model overoptimization](https://openai.com/research/scaling-laws-for-reward-model-overoptimization)
3. [(Sep, 2022) Introducing Whisper](https://openai.com/research/whisper)
4. [(May, 2022) Teaching models to express their uncertainty in words](https://openai.com/research/teaching-models-to-express-their-uncertainty-in-words)
5. [(Dec, 2021) WebGPT: Improving the factual accuracy of language models through web browsing](https://openai.com/research/webgpt)
6. [(July, 2021) Introducing Triton: Open-source GPU programming for neural networks](https://openai.com/research/triton)
7. [(Jan, 2021) DALL·E: Creating images from text](https://openai.com/research/dall-e)
8. [(Jan, 2021) CLIP: Connecting text and images](https://openai.com/research/clip)
9. [(Jan, 2021) Scaling Laws for Transfer](https://arxiv.org/pdf/2102.01293.pdf)
10. [(May, 2020) Language models are few-shot learners](https://openai.com/research/language-models-are-few-shot-learners)
11. [(May, 2020) AI and efficiency](https://openai.com/research/ai-and-efficiency)
12. [(Jan, 2020) Scaling laws for neural language models](https://openai.com/research/scaling-laws-for-neural-language-models)
    - Authors study scaling laws for language models from a large-scale experiments.
      1. _Do this rule work on object detection models?_ Yes, but the solution is based emprical results and scaling on other tasks requires a lot of mannual efforts (e.g., try all experiments on microsoft COCO). 
    - They find that the cross-entropy loss scale as a power-law with model size, dataset size, and the amount of compute used for training.
      1. _scaling laws can be formulated as a mathematics formulation?_ Yes, scaling laws shows the relationship between testing loss ($L$) and the number of parameters (N) / the size of training data (D) / the computation budget (C). In specific,
         - $$L(N)=(N_{C}/N)^{\alpha_{N}}$$
         - $$L(D)=(D_{C}/D)^{\alpha_{D}}$$
         - $$L(C)=(C_{C}/C)^{\alpha_{C}}$$
    - These findings let us determine the optimal allocation of a fixed compute budget.
      1. _How to achieve this goal?_ Given a fixed $C$, we can infer the lower bound of testing loss via $L(C)=(C_{C}/C)^{\alpha_{C}}$. Then, xxx. It shows that training a large-scale model with a few iterations is a better choice than training a small model with more iterations.
      2. _If training resource is a constant, can we predict the training loss? If yes, can we use it to infer the best training configs?_ Yes, but it requires a lot efforts in offline stages. The best training config is hard to find via scaling laws only and the searching cost is also ignored in all experiments.
13. [(2023) Compression for AGI](https://www.youtube.com/watch?v=dO4TPJkeaaU)
## Microsoft Research
1. [(EuroSys'22) Varuna: Scalable, Low-cost Training of Massive Deep Learning Models](https://www.microsoft.com/en-us/research/publication/varuna-scalable-low-cost-training-of-massive-deep-learning-models/)
2. [(NSDI'23) RECL: Responsive Resource-Efficient Continuous Learning for Video Analytics](https://www.microsoft.com/en-us/research/publication/recl-responsive-resource-efficient-continuous-learning-for-video-analytics/)
3. [(arXiv'23) Language Is Not All You Need: Aligning Perception with Language Models](https://www.microsoft.com/en-us/research/publication/language-is-not-all-you-need-aligning-perception-with-language-models/)
4. [(NeurIPS'22) M³ViT: Mixture-of-Experts Vision Transformer for Efficient Multi-task Learning with Model-Accelerator Co-design](https://www.microsoft.com/en-us/research/publication/m%c2%b3vit-mixture-of-experts-vision-transformer-for-efficient-multi-task-learning-with-model-accelerator-co-design/)
5. [(NeurIPS'22) Coarse-to-Fine Vision-Language Pre-training with Fusion in the Backbone](https://www.microsoft.com/en-us/research/publication/coarse-to-fine-vision-language-pre-training-with-fusion-in-the-backbone/)
6. [(NeurIPS'22) 3DB: A Framework for Debugging Computer Vision Models](https://www.microsoft.com/en-us/research/publication/3db-a-framework-for-debugging-computer-vision-models/)
7. [(NeurIPS'22) Robustness Analysis of Video-Language Models Against Visual and Language Perturbations](https://www.microsoft.com/en-us/research/publication/robustness-analysis-of-video-language-models-against-visual-and-language-perturbations/)
8. [(NeurIPS'22) Visual Clues: Bridging Vision and Language Foundations for Image Paragraph Captioning](https://www.microsoft.com/en-us/research/publication/visual-clues-bridging-vision-and-language-foundations-for-image-paragraph-captioning/)
9. [(ACL'22) A Good Prompt Is Worth Millions of Parameters? Low-resource Prompt-based Learning for Vision-Language Models](https://www.microsoft.com/en-us/research/publication/a-good-prompt-is-worth-millions-of-parameters-low-resource-prompt-based-learning-for-vision-language-models/)
10. [(CVPR'22) CLIP-Event: Connecting Text and Images with Event Structures](https://www.microsoft.com/en-us/research/publication/clip-event-connecting-text-and-images-with-event-structures/)
11. [(CVPR'22) DETReg: Unsupervised Pretraining with Region Priors for Object Detection](https://www.microsoft.com/en-us/research/publication/detreg-unsupervised-pretraining-with-region-priors-for-object-detection/)
12. [(CVPR'22) LAFITE: Towards Language-Free Training for Text-to-Image Generation](https://www.microsoft.com/en-us/research/publication/lafite-towards-language-free-training-for-text-to-image-generation/)
13. [(CVPR'22) Unknown-Aware Object Detection: Learning What You Don’t Know from Videos in the Wild](https://www.microsoft.com/en-us/research/publication/unknown-aware-object-detection-learning-what-you-dont-know-from-videos-in-the-wild/)
14. [(CVPR'22) Swin Transformer V2: Scaling Up Capacity and Resolution](https://www.microsoft.com/en-us/research/publication/swin-transformer-v2-scaling-up-capacity-and-resolution/)
15. [(CVPR'22) Semantic-aligned Fusion Transformer for One-shot Object Detection](https://www.microsoft.com/en-us/research/publication/semantic-aligned-fusion-transformer-for-one-shot-object-detection/)
16. [(CVPR'22) Pyramid Adversarial Training Improves ViT Performance](https://www.microsoft.com/en-us/research/publication/pyramid-adversarial-training-improves-vit-performance/)
17. [(CVPR'22) Mobile-Former: Bridging MobileNet and Transformer](https://www.microsoft.com/en-us/research/publication/mobile-former-bridging-mobilenet-and-transformer/)
18. [(CVPR'22) Debiased Learning from Naturally Imbalanced Pseudo-Labels](https://www.microsoft.com/en-us/research/publication/debiased-learning-from-naturally-imbalanced-pseudo-labels/)
19. [(NeurIPS'22) K-LITE: Learning Transferable Visual Models with External Knowledge](https://www.microsoft.com/en-us/research/publication/k-lite-learning-transferable-visual-models-with-external-knowledge/)
20. [(CACM'22) Expressive Querying for Accelerating Visual Analytics](https://www.microsoft.com/en-us/research/publication/expressive-querying-for-accelerating-visual-analytics/)
21. [(VLDB'22) Optimizing Machine Learning Inference Queries with Correlative Proxy Models](https://www.microsoft.com/en-us/research/publication/optimizing-machine-learning-inference-queries-with-correlative-proxy-models/)
22. [(SIGMOD'22) In-Database Machine Learning with CorgiPile: Stochastic Gradient Descent without Full Data Shuffle](https://www.microsoft.com/en-us/research/publication/in-database-machine-learning-with-corgipile-stochastic-gradient-descent-without-full-data-shuffle/)
23. [(TOCHI'22) What Did My AI Learn? How Data Scientists Make Sense of Model Behavior](https://www.microsoft.com/en-us/research/publication/what-did-my-ai-learn-how-data-scientists-make-sense-of-model-behavior/)
24. [(SIGMOD'22) End-to-end Optimization of Machine Learning Prediction Queries](https://www.microsoft.com/en-us/research/publication/end-to-end-optimization-of-machine-learning-prediction-queries/)
25. [(NSDI'23) GEMEL: Model Merging for Memory-Efficient, Real-Time Video Analytics at the Edge](https://www.microsoft.com/en-us/research/publication/gemel-model-merging-for-memory-efficient-real-time-video-analytics-at-the-edge-2/)
26. [(NSDI'23) SelfTune: Tuning Cluster Managers](https://www.microsoft.com/en-us/research/publication/selftune-tuning-cluster-managers/)
27. [(NSDI'23) Tambur: Efficient loss recovery for videoconferencing via streaming codes](https://www.microsoft.com/en-us/research/publication/tambur/)
28. [(ASPLOS'23) ElasticFlow: An Elastic Serverless Training Platform for Distributed Deep Learning](https://www.microsoft.com/en-us/research/publication/elasticflow-an-elastic-serverless-training-platform-for-distributed-deep-learning/)
29. [(Dec, 2022) A Study on the Intersection of GPU Utilization and CNN Inference](https://www.microsoft.com/en-us/research/publication/a-study-on-the-intersection-of-gpu-utilization-and-cnn-inference/)
30. [(SenSys'22) Turbo: Opportunistic Enhancement for Edge Video Analytics](https://www.microsoft.com/en-us/research/publication/turbo-opportunistic-enhancement-for-edge-video-analytics/)
31. [(VLDB'22) Harmony: Overcoming the hurdles of GPU memory capacity to train massive DNN models on commodity servers](https://www.microsoft.com/en-us/research/publication/harmony-overcoming-the-hurdles-of-gpu-memory-capacity-to-train-massive-dnn-models-on-commodity-servers/)
32. [(SIGCOMM'22) Genet: Automatic Curriculum Generation for Learning Adaptation in Networking](https://www.microsoft.com/en-us/research/publication/genet/)
33. [(OSDI'22) Looking Beyond GPUs for DNN Scheduling on Multi-Tenant Clusters](https://www.microsoft.com/en-us/research/publication/synergy-looking-beyond-gpus-for-dnn-scheduling-on-multi-tenant-clusters/)
34. [(ATC'22) PilotFish: Harvesting Free Cycles of Cloud Gaming with Deep Learning Training](https://www.microsoft.com/en-us/research/publication/pilotfish-harvesting-free-cycles-of-cloud-gaming-with-deep-learning-training/)
35. [(OSDI'22) Roller: Fast and Efficient Tensor Compilation for Deep Learning](https://www.microsoft.com/en-us/research/publication/roller-fast-and-efficient-tensor-compilation-for-deep-learning/)
36. [(Jul, 2022) Tutel: Adaptive Mixture-of-Experts at Scale](https://www.microsoft.com/en-us/research/publication/tutel-adaptive-mixture-of-experts-at-scale/)
37. [(MobiSys'22) CoDL: Efficient CPU-GPU Co-execution for Deep Learning Inference on Mobile Devices](https://www.microsoft.com/en-us/research/publication/codl-efficient-cpu-gpu-co-execution-for-deep-learning-inference-on-mobile-devices/)
38. [(ESEC/FCE'20) Estimating GPU memory consumption of deep learning models](https://dl.acm.org/doi/10.1145/3368089.3417050)
39. [(NSDI'23) On Modular Learning of Distributed Systems for Predicting End-to-End Latency](https://www.usenix.org/conference/nsdi23/presentation/liang-chieh-jan)
40. [(NSDI'23) Sketchovsky: Enabling Ensembles of Sketches on Programmable Switches](https://www.usenix.org/conference/nsdi23/presentation/namkung)
41. [(NSDI'23) Bamboo: Making Preemptible Instances Resilient for Affordable Training of Large DNNs](https://www.usenix.org/conference/nsdi23/presentation/thorpe)
42. [(NSDI'23) ARK: GPU-driven Code Execution for Distributed Deep Learning](https://www.usenix.org/conference/nsdi23/presentation/hwang)
## Google Research
1. [(CVPR'23) A New Path: Scaling Vision-and-Language Navigation with Synthetic Instructions and Imitation Learning](https://ai.facebook.com/research/publications/detecting-twenty-thousand-classes-using-image-level-supervision/)
2. [(ICLR'23) A New Path: Scaling Vision-and-Language Navigation with Synthetic Instructions and Imitation Learning](https://research.google/pubs/pub52240/)
3. [(TPAMI'23) Learning good features to transfer across tasks and domains](https://research.google/pubs/pub52095/)
4. [(CVPR'23) Rethinking Video ViTs: Sparse Video Tubes for Joint Image and Video Learning](https://research.google/pubs/pub52239/)
5. [(ICLR'23) Teacher Guided Training: An Efficient Framework for Knowledge Transfer](https://research.google/pubs/pub52113/)
6. [(ICLR'23) TEMPERA: Test-Time Prompt Editing via Reinforcement Learning](https://research.google/pubs/pub52083/)
7. [(CVPR'23) You Need Multiple Exiting: Dynamic Early Exiting for Accelerating Unified Vision Language Model](https://research.google/pubs/pub52223/)
8. [(ICLR'22) A Loss Curvature Perspective On Training Instability in Deep Learning](https://research.google/pubs/pub51103/)
9. [AIOps in Google Cloud](https://research.google/pubs/pub51442/)
10. [(OSDI 22) Alpa: Automating Inter- and Intra-Operator Parallelism for Distributed Deep Learning](https://research.google/pubs/pub51623/)
11. [(CVPR'22) Which Model to Transfer? Finding the Needle in the Growing Haystack](https://research.google/pubs/pub51314/)
12. [(ICML'22 Workshop) What can we do with just the model? A simple knowledge extraction framework](https://research.google/pubs/pub51476/)
13. [(NeurIPS'22) Visual Prompting via Image Inpainting](https://research.google/pubs/pub52044/)
14. [(PR'22) Towards Robust Explanations for Deep Neural Networks](https://research.google/pubs/pub50578/)
15. [(CVPR'22) Transferability Metrics for selecting Source Model Ensembles](https://research.google/pubs/pub51283/)
16. [(CVPR'22) Scaling Vision Transformers](https://research.google/pubs/pub51524/)
17. [(arXiv'22) PaLM: Scaling Language Modeling with Pathways](https://research.google/pubs/pub51308/)
18. [(MLSys'22) Pathways: Asynchronous Distributed Dataflow for ML](https://research.google/pubs/pub51473/)
19. [(CVPR'22) Proper Reuse of Image Classification Features Improves Object Detection](https://research.google/pubs/pub51359/)
20. [(NeurIPS'22 worshop) Rethinking Testing of Machine Learned Models](https://research.google/pubs/pub51392/)
21. [(NeurIPS'22) Revisiting Neural Scaling Laws in Language and Vision](https://research.google/pubs/pub51667/)
22. [(ICML'22) Model soups: averaging weights of multiple fine-tuned models improves accuracy without increasing inference time](https://research.google/pubs/pub51508/)
23. [(ICML'22) Large Batch Experience Replay](https://research.google/pubs/pub51400/)
24. [(CVPR'22) Learning to prompt for continual learning](https://research.google/pubs/pub51275/)
25. [(ICLR'22) ExT5: Towards Extreme Multi-Task Scaling for Transfer Learning](https://research.google/pubs/pub51095/)
26. [(PMLR'22) Head2Toe: Utilizing Intermediate Representations for Better Transfer Learning](https://research.google/pubs/pub51551/)
27. [(ECCV'22) How stable are Transferability Metrics evaluations?](https://research.google/pubs/pub51516/)
28. [(EMNLP'22) CPL: Counterfactual Prompt Learning for Vision and Language Models](https://research.google/pubs/pub51809/)
29. [(arXiv'22) Deduplicating Training Data Makes Language Models Better](https://research.google/pubs/pub51843/)
30. [(RL'22) Do As I Can, Not As I Say: Grounding Language in Robotic Affordances](https://research.google/pubs/pub51647/)
31. [(ECCV'22) DualPrompt: Complementary Prompting for Rehearsal-free Continual Learning](https://research.google/pubs/pub51707/)
32. [(ICLR'22) Effect of scale on catastrophic forgetting in neural networks](https://research.google/pubs/pub51163/)
33. [(CV4ARVR'22) Efficient Heterogeneous Video Segmentation at the Edge](https://research.google/pubs/pub51390/)
34. [(TMLR'22) CoCa: Contrastive Captioners are Image-Text Foundation Models](https://research.google/pubs/pub51452/)
35. [(ACM TACO, 2022) Autotuning Convolutions is Easier Than You Think](https://research.google/pubs/pub51856/)
36. [(2022) Architecture Matters in Continual Learning](https://arxiv.org/pdf/2202.00275.pdf)
37. [(2022) Scaling Laws vs Model Architectures: How does Inductive Bias Influence Scaling?](https://arxiv.org/pdf/2207.10551.pdf)
38. [(2021) Efficient Deep Learning: A Survey on Making Deep Learning Models Smaller, Faster, and Better](https://arxiv.org/pdf/2106.08962.pdf)
39. [(NSDI'23) HALP: Heuristic Aided Learned Preference Eviction Policy for YouTube Content Delivery Network](https://www.usenix.org/conference/nsdi23/presentation/song-zhenyu)
40. [(arXiv'22) Preserving In-Context Learning ability in Large Language Model Fine-tuning](https://arxiv.org/abs/2211.00635)
## Meta AI
### Foundation models
1. [(CVPR'23) Segment Anything](https://ai.facebook.com/research/publications/segment-anything/) [Github](https://github.com/facebookresearch/segment-anything)![Github stars](https://img.shields.io/github/stars/facebookresearch/segment-anything)
2. [(NeurIPS'22) Neural Attentive Circuits](https://ai.facebook.com/research/publications/neural-attentive-circuits/)
3. [(ECCV'22) Three things everyone should know about Vision Transformers](https://ai.facebook.com/research/publications/three-things-everyone-should-know-about-vision-transformers/)
4. [(Yann Lecun, 2022) A Path Towards Autonomous Machine Intelligence](https://openreview.net/pdf?id=BZ5a1r-kVsf&utm_source=pocket_mylist) ([video](https://www.buffalo.edu/ai-data-science/news-events/events/speakers.host.html/content/shared/www/ai-data-science/DSS/lecun.detail.html))
5. [(CVPR'23) ImageBind: One Embedding Space To Bind Them All](https://facebookresearch.github.io/ImageBind/paper) [Github](https://github.com/facebookresearch/ImageBind)![Github stars](https://img.shields.io/github/stars/facebookresearch/ImageBind)
6. [(CVPR'23 highlight) Learning Video Representations from Large Language Models](http://arxiv.org/abs/2212.04501) [Github](https://github.com/facebookresearch/LaViLa)![Github stars](https://img.shields.io/github/stars/facebookresearch/LaViLa)
7. [(arXiv, 2023) Learnings from Data Integration for Augmented Language Models](https://research.facebook.com/publications/learnings-from-data-integration-for-augmented-language-models/)
8. [(arXiv, 2023) Effective Theory of Transformers at Initialization](https://research.facebook.com/publications/effective-theory-of-transformers-at-initialization/)
9. [(arXiv, 2023) LLaMA: Open and Efficient Foundation Language Models](https://research.facebook.com/publications/llama-open-and-efficient-foundation-language-models/)
10. [(ICLR'23) Progressive Prompts: Continual Learning for Language Models](https://research.facebook.com/publications/progressive-prompts-continual-learning-for-language-models/)
### Open-vocabulary
1. [(ECCV'22) Detecting Twenty-thousand Classes using Image-level Supervision](https://ai.facebook.com/research/publications/detecting-twenty-thousand-classes-using-image-level-supervision/)![Github stars](https://img.shields.io/github/stars/facebookresearch/Detic)
2. [(ICLR'23) Building a Subspace of Policies for Scalable Continual Learning](https://research.facebook.com/publications/building-a-subspace-of-policies-for-scalable-continual-learning/)
### Scaling laws and benchmarks
1. [(NeurIPS'22) Beyond neural scaling laws: beating power law scaling via data pruning](https://ai.facebook.com/research/publications/beyond-neural-scaling-laws-beating-power-law-scaling-via-data-pruning/)
2. [(ICLR'23) ImageNet-X: Understanding Model Mistakes with Factor of Variation Annotations](https://research.facebook.com/publications/imagenet-x-understanding-model-mistakes-with-factor-of-variation-annotations/)
### Edge-AI
1. [(TOSEM'23) ArchRepair: Block-Level Architecture-Oriented Repairing for Deep Neural Networks](https://ai.facebook.com/research/publications/archrepair-block-level-architecture-oriented-repairing-for-deep-neural-networks/)
2. [(TPDS'22) TFormer: A Transmission-Friendly ViT Model for IoT Devices](https://ai.facebook.com/research/publications/tformer-a-transmission-friendly-vit-model-for-iot-devices/)
3. [(ICLR'23) Token Merging: Your ViT but Faster](https://github.com/facebookresearch/ToMe)
4. [(2020) PySlowFast: open source video understanding codebase](https://github.com/facebookresearch/SlowFast)![Github stars](https://img.shields.io/github/stars/facebookresearch/SlowFast)
5. [(MM'21) PyTorchVideo: A Deep Learning Library for Video Understanding](https://github.com/facebookresearch/pytorchvideo)![Github stars](https://img.shields.io/github/stars/facebookresearch/pytorchvideo)
6. [Mobile Computer Vision @ Facebook](https://github.com/facebookresearch/mobile-vision)![Github stars](https://img.shields.io/github/stars/facebookresearch/mobile-vision)
7. [(TinyML'23) Design and analysis of hardware friendly pruning algorithms to accelerate deep neural networks at the edge](https://research.facebook.com/publications/design-and-analysis-of-hardware-friendly-pruning-algorithms-to-accelerate-deep-neural-networks-at-the-edge/)
### Algorithm-system co-design
1. [(NSDI'23) TopoOpt: Co-optimizing Network Topology and Parallelization Strategy for Distributed Training Jobs](https://www.usenix.org/conference/nsdi23/presentation/wang-weiyang)
2. [(NSDI'23) Better Together: Jointly Optimizing ML Collective Scheduling and Execution Planning using SYNDICATE](https://www.usenix.org/conference/nsdi23/presentation/mahajan)
3. [(HiPC'23) Building a Performance Model for Deep Learning Recommendation Model Training on GPUs](https://research.facebook.com/publications/building-a-performance-model-for-deep-learning-recommendation-model-training-on-gpus/)
4. [(CLOUD'23) Serving distributed inference deep learning models in serverless computing](https://research.facebook.com/publications/serving-distributed-inference-deep-learning-models-in-serverless-computing/)