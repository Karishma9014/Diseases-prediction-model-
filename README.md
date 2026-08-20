# Diseases-prediction-model-
Disease Prediction Model is a machine-learning program that predicts a possible disease based on symptoms entered by the user. It can be used as an educational project to demonstrate classification using Python; it is not a substitute for a doctor's diagnosis.
# Disease Prediction Model
# Educational example

print("=== Disease Prediction Model ===")

fever = input("Do you have fever? (yes/no): ").lower()
cough = input("Do you have cough? (yes/no): ").lower()
headache = input("Do you have headache? (yes/no): ").lower()
stomach_pain = input("Do you have stomach pain? (yes/no): ").lower()

if fever == "yes" and cough == "yes":
    disease = "Possible Flu-like illness"
elif fever == "yes" and headache == "yes":
    disease = "Possible viral illness"
elif stomach_pain == "yes" and fever == "yes":
    disease = "Possible stomach infection"
elif cough == "yes":
    disease = "Possible respiratory illness"
else:
    disease = "No clear prediction"

print("\nPrediction:", disease)
print("Note: This is only an educational prediction, not a medical diagnosis.")
