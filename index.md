## CORAL (Curve resOlution foR data AnaLysis

CORAL is a set of chemometrics tools built in Python to perform multivariate spectral decomposition of large amount of XAS data. These tools are implemented in Jupyter Notebook and allow users to overcome difficulties related to the huge amount of data coming from fast data acquisition during time-resolved XAS studies. On beamlines controlled by Jupyter environment, such as the future XAS beamline at SIRIUS, it also permits the creation of a complete experimental Notebook that allows to get on track the data analysis.

### MCR-ALS:
#### What is MCR-ALS?

Multivariate Curve Resolution with Alternating Least Squares (MCR-ALS) is a powerful chemometric tool to solve mixture problems. This method has been applied to different techniques to obtain the relative concentration profiles (**C**) and the pure spectra ($𝐒^𝐓$). The main idea of MCR-ALS is to decompose the original data matrix (**D**), the decomposition must be as: **$𝐃=𝐂𝐒^𝐓 + E$** (eq. 1). Where (**E**) is the matrix of the residuals.
Combined with constraints MCR-ALS can obtain results that obey the behavior of the studied system. Besides, our implementation in Python allows users to use GPU acceleration.

For TR-XAS data the **equation 1** must be transposed so: **$D^T = (CS^T)^T = SC^T$**, in this sense, the spectra must be displayed in a row-format, this means that each column is a different energy (wavelenght).
