# **Intelligent Shipping Cost Calculation Using LLM and Chatbot**
## Overview
This project demonstrates an intelligent shipping cost calculation system, integrated with a chatbot, that interacts with users to provide accurate shipping costs based on product dimensions, weight, and delivery location. The system dynamically adjusts costs for metro/non-metro areas, oversized items, and non-deliverable locations.

## **Features**
* **Chatbot Interface**: Interacts with users to get product details and delivery location.
* **Dynamic Cost Calculation**: Computes shipping cost based on length, breadth, height, and weight of the product.
* **Metro/Non-Metro Adjustments**: Applies lower rates for metro deliveries and additional charges for non-metro areas.
* **Oversized Product Handling**: Adds extra fees for products exceeding 2 feet in height or 8 kg in weight.
* **Error Handling**: Provides appropriate feedback for non-deliverable pincodes.
  
## **Technologies Used**
* **Python**: Backend and data handling.
* **Flask**: REST API implementation for chatbot interactions and cost calculation.
* **TensorFlow**: LLM training using the GPT-2 model.
* **Hugging Face Transformers**: For fine-tuning and implementing GPT-2.
* **Pandas**: For handling and processing product data (CSV files).
  
## **Installation**
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/intelligent-shipping-cost-calculator.git
2. Install the required dependencies:
    ```bash
    pip install -r requirements.txt

4. Prepare your dataset (product dimensions and weights) in a CSV file and ensure it is in the expected format.

5. Run the Flask server:
   ```bash
    python app.py

## **Usage**
1. Interact with the chatbot by providing the product name and delivery pincode.
2. The system will compute and return the shipping cost based on the provided data.
3. If the pincode is non-deliverable or the product exceeds size limits, appropriate feedback will be given.

## **File Structure**
* fine_tuned_gpt2/: Directory containing the fine-tuned GPT-2 model.
* metro_pincodes.csv: File containing a list of metro city pincodes.
* same_city_pincodes.csv: File containing a list of all pincodes of Pune.
* product_data.csv: CSV file with product dimensions (length, breadth, height, weight).

## **Contributions**
Feel free to contribute by forking the repository and submitting a pull request.

## **Conclusion**

This project demonstrates the integration of a chatbot with an intelligent shipping cost calculator powered by a fine-tuned GPT-2 model. By utilizing product dimensions, weights, and delivery pincodes, the system dynamically calculates shipping costs, applying additional charges for non-metro areas and oversized items. The flexibility and accuracy of the model make it adaptable for various shipping scenarios, enhancing customer experience and streamlining logistics operations. With the use of modern technologies like Flask, TensorFlow, and Transformers, this application highlights the potential of AI in automating complex, real-world tasks.
