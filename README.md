# Java ATM Simulator

Welcome to the Java ATM Simulator repository! This project aims to simulate the functionality of an Automated Teller Machine (ATM) using Java and Java Swing/AWT. It provides a user-friendly interface for performing various banking transactions such as withdrawals, deposits, balance inquiries, and more.

## Overview

The Java ATM Simulator offers the following functionality:

### PIN Authentication

![PIN Authentication](https://github.com/Baniya-sen/ATM-Working-Simulation/assets/144620117/ce4c1c3f-2160-44a0-86a1-e8a6ef3abb8e)



- **Description**: The ATM simulator features a secure PIN authentication system to verify the identity of the user. Users are required to enter their unique PIN (Personal Identification Number) to access their accounts and perform transactions. The PIN authentication process ensures the security and confidentiality of the user's banking information.

### Account Balance Inquiry

![Balance Inquiry](https://github.com/Baniya-sen/ATM-Working-Simulation/assets/144620117/628862bb-2229-4359-b752-e199fd3ff770)



- **Description**: Users can check their account balances conveniently using the ATM simulator. Upon successful authentication, the system displays the current balance of the user's account, providing them with real-time financial information.

### Cash Withdrawal

![Cash Withdrawal](https://github.com/Baniya-sen/ATM-Working-Simulation/assets/144620117/e3e7cf56-729b-4004-b21f-6a5e178ee568)



- **Description**: The ATM simulator allows users to withdraw cash from their accounts quickly and efficiently. Users can specify the desired withdrawal amount, and the system deducts the corresponding funds from their account balance.

### Cash Deposit

![Cash Deposit](https://github.com/Baniya-sen/ATM-Working-Simulation/assets/144620117/c0c9bf3e-1e67-4be6-aadf-ff6898bf14c9)



- **Description**: Users can deposit cash into their accounts using the ATM simulator. Simply insert the desired amount of cash into the designated slot, and the system adds the deposited funds to the user's account balance.


## Usage

1. **Launch the Application**: Run the `Main.java` file to launch the ATM simulator application.
   The main file contains code-
   
   ```Java
      import javax.swing.*;
    
      public class Main {
      
          public static void main(String[] args) {
              SwingUtilities.invokeLater(Welcome_UI::new);
          }
      }```
   
2. **PIN Authentication**: Enter any PIN (for now!) using the on-screen keypad to authenticate your identity.
3. **Perform Transactions**: Choose from the available options to perform transactions such as balance inquiry, cash withdrawal, cash deposit, and fund transfer.
4. **Follow On-Screen Prompts**: Follow the on-screen prompts to complete each transaction successfully.
5. You can adjust key presses functionality in `ATM_ButtonListeners` file where the key method is-
   ```Java
      @Override
      public void keyReleased (KeyEvent e){
  
          final int letterAKeycode = 65;
          if (e.getKeyCode() == letterAKeycode) {
              actionPerformed(new ActionEvent(atmUi.screenButtons[1], ActionEvent.ACTION_PERFORMED, null));
          }```


## Contributions

Contributions to the Java ATM Simulator project are welcome! If you have any suggestions for additional features, improvements, or bug fixes, feel free to submit a pull request or open an issue on GitHub.

Thank you for using the Java ATM Simulator. We hope you find it useful for simulating various banking transactions and learning about ATM functionality in Java.
