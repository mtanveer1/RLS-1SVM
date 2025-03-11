# RLS-1SVM - Enhancing robustness and sparsity: least squares one-class support vector machine

This code corresponds to the paper: Anuradha Kumari, M. Tanveer. "Enhancing robustness and sparsity: least squares one-class support vector machine. https://dx.doi.org/10.2139/ssrn.5095202”

If you are using our code, please give proper citation to the above given paper.

%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%

We have put a demo of the "RLS_1SVM" and "SRLS_1SVM" models with the “breast_cancer_wisc_diag” dataset.

Description of files:

RLS_OCSVM_main: This is the main file of RLS_1SVM. To utilize the code, you simply need to import the data and execute this script. Within the script, it tunes various parameters of the model (regularization hyperparameter: C_1,C_2, and kernel parameter: sigma). To replicate the results achieved with RLS_1SVM, you should adhere to the same instructions outlined in the paper.

SRLS_OCSVM_main: This is the main file of SRLS_1SVM. To utilize the code, you simply need to import the data and execute this script. Within the script, it tunes various parameters of the model (regularization hyperparameter: C_1,C_2, kernel parameter: sigma, and rank parameter: r). To replicate the results achieved with SRLS_1SVM, you should adhere to the same instructions outlined in the paper.

RLS_OCSVM_func: The RLS_OCSVM_main calls this file for the training. It contains the function of solving the  optimization problem of proposed RLS_1SVM algorithm.

SRLS_OCSVM_func: The SRLS_OCSVM_main file calls this file for the training. It contains the function of solving the  optimization problem of proposed SRLS_1SVM algorithm.


Evaluate: This function calculates G-mean using the true and predicted label.

kernelfun: This is the kernel function utilized to map the data points to kernel space using RBF kernel. 

RLS_OCSVM_test_model1:This function predicts labels for training data using the RLS_1SVM model.
RLS_OCSVM_test_model2: This function predicts labels for validation data using the RLS_1SVM model.
RLS_OCSVM_test_model3: This function predicts labels for test data using the RLS_1SVM model.

test_model1_SRLS_OCSVM: This function predicts labels for training data using the SRLS_1SVM model.
test_model2_SRLS_OCSVM: This function predicts labels for validation data using the SRLS_1SVM model.
test_model3_SRLS_OCSVM: This function predicts labels for test data using the SRLS_1SVM model.

The codes are not optimized for efficiency. The codes have been cleaned for better readability and are the same as used in our paper. For the detailed experimental setup, please follow the paper. We have re-run and checked the codes only in a few datasets, so if you find any bugs/issues, please write to Anuradha Kumari (phd2101141007@iiti.ac.in).

