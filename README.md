# Pixel Diagnose

Welcome to Pixel Diagnose! 🧠 Our mission is to empower radiologists with state-of-the-art artificial intelligence, enhancing the accuracy of differential diagnoses for cancer patients.

## How It Works

Pixel Diagnose acts as a clinician's digital assistant, employing an advanced architecture to boost diagnostic precision. Imagine a radiologist examining a brain scan of a potential tumor patient, seeking confirmation by comparing it with other patients' scans. Unlike a human, our application can scan through thousands of MRI images in seconds. We enable the comparison of a patient’s MRI scan with numerous similar images across various diagnoses. This process involves embedding query images and employing cosine similarity in our vector store for precise matching, followed by retrieving similar images from our extensive database.

[Demo Video](https://github.com/pixel-diagnose/.github/assets/75021486/cca21087-eb2b-4be6-85b2-3bdd8e64d5c5)

## Quick Start
Get started with our Docker image:
1. `docker pull mkstatistics/pixel-diagnose-demo`
2. `docker run -d -p 5001:5001 mkstatistics/pixel-diagnose-demo`
3. Open [http://127.0.0.1:5001](http://127.0.0.1:5001) and explore the project.

## Features 🧠

- **Query Image Input**: Upload an MRI image and receive similar images from our database.
- **Segmentation Options**: Choose between whole brain or tumor-segmented images.
- **Multiple MRI Modalities**: Work with various MRI modalities (T1, T1 with contrast, T2, Flair) for a more nuanced diagnosis.

## Technology

In our current demo, we primarily employ the RESNet50 model from the Imagenet-pretrained CNN series. This model has been selected for its proven reliability and efficiency in image analysis. Alongside the RESNet50, we are actively experimenting with other advanced models, including MedClip (RESNet50 and Swin Transformer), finetuned EfficientNetV2, and a custom CNN with Triplet Loss. All our models, including those in the experimentation phase, are undergoing extensive evaluation. This process includes expert ratings and internal assessments to ensure the highest levels of reliability and accuracy in our diagnostic tools.

## Current Scope

Our current proof of concept effectively supports differential diagnosis for three brain tumor types: glioma, meningioma, and metastasis.

## Future

Pixel Diagnose is committed to expanding its impact beyond brain tumor diagnosis. Our current focus includes embedding and similarity search for 2D brain scan slices. The next major step is to implement similarity search based on 3D segmentations and embeddings. This advancement will not only enhance our brain tumor diagnostics but also lay the groundwork for applying our technology to various other types of tumors, broadening our scope and impact in the field of radiology.

## Developer Resources

Explore our repositories:

- [pixel-diagnose](https://github.com/pixel-diagnose/pixel-diagnose): Development notebooks on visualization, segmentation, models, qdrant vector database, cloud communication.
- [user-app-frontend](https://github.com/pixel-diagnose/user-app-frontend): Frontend application built using React and Vite.
- [user-application](https://github.com/pixel-diagnose/user-application): Flask backend framework, Dockerfile, Static and Templates Directories for Interface.

## Contributing

Join us in our mission to revolutionize radiology diagnostics! We welcome contributions in the form of code, ideas, or feedback.

## Contact

Connect with our team:
- [Michael Gerloff](https://www.linkedin.com/in/michael-gerloff/)
- [Svenja Niehaus](https://www.linkedin.com/in/svenja-niehus/)
- [Dr. Katja Dittrich](https://www.linkedin.com/in/katja-dittrich/)
- [Antonio Rueda-Toicen](https://www.linkedin.com/in/antonioruedatoicen/)

## License

Pixel Diagnose is open-sourced under the [GNU Affero GPL v3 License](LICENSE.md).

## Support
For support, please open an issue or contact us at [pixeldiagnose@gmail.com](mailto:pixeldiagnose@gmail.com).

---

*Empowering Radiologists, One Pixel at a Time.* 🧠💡
