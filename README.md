**College Admission Smart Contract**

**Introduction:**

This repository contains a Solidity smart contract for managing college admissions. The contract is designed to facilitate the admission process for students applying to a college, including selection rounds and seat allocation based on predefined criteria.

**Smart Contract Overview:**

The `CollegeAdmission` contract includes functions to manage the admission process, handle seat selection rounds, and allocate seats to eligible candidates. Below is a brief overview of the contract functionalities:

1. **Total Students Counter:**
    - `totalStudents`: A public variable to track the total number of students admitted to the college.

2. **Reserved Seats:**
    - `reservedSeatsXandY`: A public variable representing the number of reserved seats for a specific category (X and Y).

3. **Admission Process:**
    - `admissionProcess(uint256 _numStudents)`: External function to initiate the admission process by specifying the number of students applying. It asserts that the number of students should be greater than a predefined threshold.

4. **Selection Rounds:**
    - `selectionRound1(string memory _category)`: External pure function to conduct the first selection round based on the category provided. It verifies if the provided category is eligible for seat allocation.
    - `SelectionRound2(string memory _category)`: External function for the second selection round. It checks the availability of reserved seats and allocates them to eligible candidates based on the category. If the criteria are not met, it reverts with a custom error message.

**License:**

This smart contract is licensed under the MIT License. See the SPDX-License-Identifier tag within the contract for more details.

## Author 

Yogimani shree

blue2321@gmail.com


