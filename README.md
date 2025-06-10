#PBMC Single-Cell CITE-seq, RNA + ADT

Project Overview
This project analyzes peripheral blood mononuclear cells (PBMCs) from a clinical study using single-cell CITE-seq (RNA + surface protein) data. The goal is to characterize common and rare immune cell types by integrating transcriptomic and surface marker information, enabling a comprehensive view of immune cell diversity within human blood samples.

---

## 📊 Analysis Tasks

### **Task 1: Data Loading, QC, and Visualization**
- Created individual Seurat objects for each sample and a combined object.
- Performed quality control on RNA and ADT modalities
- Visualized key metrics (e.g., gene count, mitochondrial percent)

### **Task 2: Independent RNA and Protein Integration**
- **RNA assay**: Normalization, CCA-based integration, scaling, and PCA  
- **Protein (ADT) assay**: CLR normalization, integration, scaling, and PCA  
- Addressed batch effects within each modality prior to multimodal combination

### **Task 3: WNN Integration, Clustering, and Annotation**
- Combined RNA and protein PCA using Seurat's Weighted Nearest Neighbors (WNN)
- Generated UMAP and t-SNE plots on multimodal space
- Identified and annotated clusters using canonical immune markers

### **Task 4: Gene Feature Extraction and Visualization**
- Extracted gene expression values for specific genes
- Added gene features to Seurat metadata
- Visualized expression patterns per cell type per Group

---


## 💡 Notes

- Raw data is not publicly available due to client ownership and confidentiality.
- Some example outputs plots are organized by task in the `output/` folder.
- This project is designed for both reproducibility and clarity.

---

## 📬 Contact

*Author:* Nasim Rahmatpour 
*Email:* nasimrahmatpour1@gmail.com 
*GitHub:* (https://github.com/nasimbio)
