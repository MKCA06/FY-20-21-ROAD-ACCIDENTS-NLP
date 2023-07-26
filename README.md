<!DOCTYPE html>
<html>
<head>
    <title>FY 20-21 Road Accidents Classification Project</title>
</head>
<body>
    <header>
        <h1>FY 20-21 Road Accidents Classification Project</h1>
    </header>

    <main>
        <section>
            <h2>Project Overview</h2>
            <p>This repository contains code and data related to a project involving road accidents in the fiscal year 2020-2021. The main goal of the project is to classify the direct cause and category of the accidents using Natural Language Processing (NLP) techniques.</p>
        </section>

        <section>
            <h2>Dataset</h2>
            <p>The dataset used for this project contains information about road accidents that occurred during the FY 20-21. It includes the following columns:</p>
            <ul>
                <li>S.No: Serial number of the accident record.</li>
                <li>DIV: Division code.</li>
                <li>Deptt: Department code.</li>
                <li>Employee type: Type of employee involved in the accident.</li>
                <li>Date: Date of the accident.</li>
                <li>Injury: Description of injuries sustained by the individuals involved in the accident.</li>
                <li>Fracture: Indicates whether there was a fracture (Yes/No).</li>
                <li>Details: Detailed information about the accident.</li>
                <li>Category: Category of the accident.</li>
                <li>Direct Cause: Direct cause of the accident.</li>
            </ul>
        </section>

        <section>
            <h2>Code</h2>
            <p>The project code is written in Python and involves various NLP techniques to extract and classify relevant information from the "Details" column of the dataset. Below are some of the key functions used in the code:</p>
            <ul>
                <li>extract_transport_mode(text): Extracts the mode of transport involved in the accident from the given text.</li>
                <li>extract_direct_cause(text): Identifies the direct cause of the accident from the provided text.</li>
                <li>extract_location2(text): Extracts the location of the accident from the given text using entity recognition (GPE - Geopolitical Entity).</li>
                <li>extract_shift(text): Identifies the shift time (A, B, C, or G) mentioned in the text.</li>
                <li>extract_time(text): Extracts any time-related information from the text.</li>
                <li>object_hinderance(text): Checks if there was any object hinderance involved in the accident.</li>
                <li>Person_fault(text): Checks if the accident was due to the fault of a person.</li>
                <li>severity_safe(text, text2): Classifies the severity of the accident based on injury and fracture information.</li>
            </ul>
            <p>The code processes the "Details" column of the dataset and creates additional columns in the dataframe to store the extracted information, such as transport mode, location, shift time, time, object hinderance, person fault, accident severity, and direct cause.</p>
        </section>

        <section>
            <h2>Usage</h2>
            <p>To use the code, follow these steps:</p>
            <ol>
                <li>Clone the repository to your local machine.</li>
                <li>Ensure you have the required libraries installed (NLTK, SpaCy with the en_core_web_lg model).</li>
                <li>Load the dataset and run the provided Python code.</li>
                <li>The code will process the "Details" column and create additional columns with extracted information.</li>
                <li>The final dataframe with the additional columns will be saved for further analysis or classification tasks.</li>
            </ol>
            <p>Feel free to explore and modify the code to suit your specific requirements and to improve the accuracy of the classification model.</p>
        </section>

        <section>
            <h2>Note</h2>
            <p>Please note that the project code is based on the available dataset and specific NLP techniques. The accuracy and performance of the classification model may vary depending on the quality of the data and the nature of the accidents recorded. For any questions or issues related to the project or the code, feel free to raise an issue or contact the repository owner.</p>
        </section>
    </main>

    <footer>
        <p>&copy; 2023 Your Organization. All rights reserved.</p>
    </footer>
</body>
</html>
