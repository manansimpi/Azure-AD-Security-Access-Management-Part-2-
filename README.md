# Azure-AD-Security-Access-Management(Part-2)
## Phase 2: Implementing Identity Protection.
### Step 1: Access Azure AD Identity Protection
- Navigate to Identity Protection from the Azure portal.

### Step 2: Configure User Risk Policy.
- In the Identity Protection dashboard, go to User Risk Policy.

 ![Screenshot 2025-01-29 224736](https://github.com/user-attachments/assets/a0b9d6fc-340d-4a97-8185-2160269a04a7)

<br><br>

- Start Creating Policies. For Lab purposes, it's a good habit to exclude the Owner of the Tenant since sometimes you could lock out yourself which would be a hassle.
  
 ![Screenshot 2025-01-29 224952](https://github.com/user-attachments/assets/ec8f74a6-6fd7-4d5b-a69f-de59ae7b91c1)

  <br><br>
  
- Granting Access to the users with Low and Above User Risk after changing Passwords. Can block their access  as well as below.
  
 ![Screenshot 2025-01-29 225309](https://github.com/user-attachments/assets/324afa6e-4116-4f23-b5d9-f81fa2586283)

 <br><br>
 
 ![Screenshot 2025-01-29 225343](https://github.com/user-attachments/assets/ad2a50d7-121b-4b81-b72f-ac01a5a9d5c8)

 <br><br>

 ![Screenshot 2025-01-29 225343](https://github.com/user-attachments/assets/f7b6fc8c-74fb-458d-b479-6996354bdeac)

 ### Step 3: Configure Sign-in Risk Policy
 - Here the configurations are similar it's just we can Allow Access to Users by Enforcing MFA(Multi-Factor Authentication) based on the Sign-in Risk Level.

![Screenshot 2025-01-29 231425](https://github.com/user-attachments/assets/90067d20-37e1-4690-ba5f-a41f40129f48)


### Step 4: Enable Multi-Factor Authentication (MFA)

- Again navigate to Identity Protection from the Azure portal.
- Click New Policy and name it MFA for High-Risk Users.

![Screenshot 2025-01-29 233023](https://github.com/user-attachments/assets/2ce9e1fc-8ec0-41d3-b3e8-c42703013570)

<br><br>

![Screenshot 2025-01-29 233510](https://github.com/user-attachments/assets/af5c1e28-cc93-46cd-8959-ba86b856332f)

<br><br>

![Screenshot 2025-01-29 233600](https://github.com/user-attachments/assets/71bb25a0-9f46-4ece-9939-1ef4b0f50723)


<br><br>

![Screenshot 2025-01-29 233735](https://github.com/user-attachments/assets/117a214e-f2a8-47f8-aea9-276b0da9431b)


<br><br>

![Screenshot 2025-01-29 233814](https://github.com/user-attachments/assets/63a62a8a-8fd6-45e7-bb1b-ed6a55042d83)


### Step 5: Simulating a Risky Sign-in (Testing)

1. Use a VPN or a new device to simulate an unfamiliar sign-in.

 ![Screenshot 2025-01-29 234348](https://github.com/user-attachments/assets/e4aeb922-0865-46d7-a7a5-d3b29ec0ac5f)

 - Since I had not configured MFA before on this account it just Locked me out.

![Screenshot 2025-01-29 234314](https://github.com/user-attachments/assets/66af7820-2c26-4fe7-8fba-4715026042dd)

<br><br>

![Screenshot 2025-01-30 000224](https://github.com/user-attachments/assets/d25d521d-ee6f-4f24-bf5b-4af1ed1164ed)


- Now let's try with the account that has MFA set up already.

 ![image](https://github.com/user-attachments/assets/c38e441c-0088-41cb-b879-38b358ae95b0)

 <br><br>

  ![Screenshot 2025-01-30 000540](https://github.com/user-attachments/assets/1cb7fa3c-ecbb-40c2-8546-4866a611e127)

- There we goooooooo.

![Screenshot 2025-01-30 000656](https://github.com/user-attachments/assets/5d46a1de-58d4-47b5-8f1d-e44d054dc1c9)


### Step 6: Monitoring Risk Events.

![Screenshot 2025-01-30 001848](https://github.com/user-attachments/assets/6f3ec28f-ac1d-49fb-93bc-1e1c2271c890)

<br><br>

![Screenshot 2025-01-30 001502](https://github.com/user-attachments/assets/1610e0b1-1ead-4ea1-8a84-d87b0e22c4a4)

<br><br>

![Screenshot 2025-01-30 001555](https://github.com/user-attachments/assets/45be0461-852d-4baa-b402-035092f2551f)
