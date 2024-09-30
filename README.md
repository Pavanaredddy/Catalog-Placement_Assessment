# Shamir_Secret_Sharing_problem.js
# Overview
This project implements Shamir's Secret Sharing algorithm, which allows a secret to be divided into parts, giving each participant its own unique part. A specified minimum number of parts (k) are required to reconstruct the original secret. This algorithm is particularly useful in scenarios requiring secure data sharing and distribution.

# Project Structure
index.js: Contains the main logic for decoding input values, implementing Lagrange interpolation, and finding both the secret and any incorrect points.
package.json: Contains project metadata and dependencies (e.g., big-integer for handling large integers).
# Features
Base Conversion: Supports converting values from various bases to decimal for easy calculations.
Lagrange Interpolation: Implements the Lagrange interpolation polynomial to calculate the secret (c).
Error Detection: Identifies points that do not conform to the expected polynomial.
# # How to Run the Project
# Prerequisites
Node.js installed on your system.
# Installation
Clone the repository to your local machine:
             git clone <repository-url>
             cd <repository-directory>
Install the required dependencies:
            npm install
            Running the Code
To execute the code, run the following command:
            node index.js
This will process the test cases defined in the code and output the secret and any incorrect points.

# Input:
The input consists of two test cases, each structured as follows:
json
{
    "keys": {
        "n": <total points>,
        "k": <minimum points needed to reconstruct the secret>
    },
    "<point_index>": {
        "base": "<base>",
        "value": "<value>"
    }
}
n: Total number of points.
k: Minimum number of points required to reconstruct the secret.
Each point is defined by its index, base, and value.
# Output:
Output for testcase 1
23
Output for testcase 2
172413718232801
Wrong points in testcase 2 in (x,y) format
(7, 28859585857715), (8, 28735619441184), (9, 28735619219333)
# Author
Pavana Maddireddy
