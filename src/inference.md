## Inference

An **inference engine** is a specialized runtime designed to execute trained models efficiently on hardware. This is made up of a trained model, which is usually in its default PyTorch (.pt), TensorFlow (.tf2) format, and a **serving framework.**

Besides parsing the inference engine and executing it, a **Serving Framework** takes care of managing the inference server. This includes system-wide optimizations, batching, request-response mapping, and more. Examples include vLLM, Ollama, BentoML, Hugging Face TGI, and others.

There is no one-size-fits-all runtime. The right choice depends on your **hardware**, your **latency** vs. **throughput** needs, and whether your model is running in the cloud or on the edge.

### Model storage formats

> You can think of it as a movie in full quality (not even the contents of the blu-ray disc, rather the edited camera footage itself), so if anyone is going to fiddle with it, it's preferred to be done with the source. GGUF, exl2 and the rest are "rips" like mp4 or mov, of various quality, which are more user-friendly for "playback". Just like the codecs, the quantization formats change sometimes, new technologies emerge to improve the efficiency, so what once was the gold standard (GGML) is now obsolete (remember DivX?)

