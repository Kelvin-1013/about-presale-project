1. **Token Program Integration**:


- The program uses CPI (Cross-Program Invocation) to interact with the Token Program 
- Token transfers are handled through CPI contexts that specify the source and destination accounts 
- The mint initialization is performed with proper authority and decimals configuration 


2. **Account Structure**:


- The presale vault acts as the main token custody account 
- Associated Token Accounts (ATAs) are created for users to receive tokens 
- The mint authority is controlled by the program for token issuance 


3. **Program Flow**:


- System Program transfers handle SOL movements for purchases 
- Token Program handles all token-related operations (minting, transfers) 
- The presale program maintains state and orchestrates the interaction between these components 


4. **Security Considerations**:


- Program-Derived Addresses (PDAs) are used for deterministic account generation
- Proper authority checks are implemented for all sensitive operations
- Token accounts are verified before transfers to prevent unauthorized access


The architecture follows Solana's best practices for token management and program composition, with clear separation between system-level operations and token-specific functionality.

Would you like me to elaborate on any specific part of these diagrams or relationships?