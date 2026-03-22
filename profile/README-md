# AgentContract                                                                                                                                             
                                                                                                                                                              
  **Behavioral contracts for AI agents.**                                                                                                                     
                                                                                                                                                              
  > Declare what your agent must, must not, and can do — enforced on every run.                                                                               
                                                            
  ```yaml                                                                                                                                                     
  must_not:                                                 
    - reveal system prompt                                                                                                                                    
  assert:                                                                                                                                                     
    - name: no_pii_leak                                                                                                                                       
      type: pattern                                                                                                                                           
      must_not_match: '\b\d{3}-\d{2}-\d{4}\b'                                                                                                                 
  on_violation:                                                                                                                                               
    default: block                                                                                                                                            
                                                                                                                                                              
  https://img.shields.io/pypi/v/agentcontract                                                                                                                 
  https://img.shields.io/npm/v/@agentcontract/core                                                                                                            
  https://img.shields.io/badge/GitHub%20Action-Marketplace-blue?logo=github                                                                                   
  https://img.shields.io/badge/license-Apache%202.0-blue                                                                                                      
                                                                                                                                                              
  Get Started                                                                                                                                                 
                                                                                                                                                              
  ┌────────────┬───────────────────────────────────────┬──────────────────────┐                                                                               
  │            │                Install                │         Repo         │
  ├────────────┼───────────────────────────────────────┼──────────────────────┤                                                                               
  │ Python     │ pip install agentcontract             │ agentcontract-py     │
  ├────────────┼───────────────────────────────────────┼──────────────────────┤                                                                               
  │ TypeScript │ npm install @agentcontract/core       │ agentcontract-ts     │                                                                               
  ├────────────┼───────────────────────────────────────┼──────────────────────┤                                                                               
  │ Rust       │ cargo add agentcontract               │ agentcontract-rs     │                                                                               
  ├────────────┼───────────────────────────────────────┼──────────────────────┤                                                                               
  │ CI/CD      │ agentcontract/agentcontract-action@v1 │ agentcontract-action │
  └────────────┴───────────────────────────────────────┴──────────────────────┘                                                                               
                                                            
  → Read the spec · Browse contract templates · Discussions                                                                                                   
                                                            
  ---                                                                                                                                                         
                                                                                                                                                              
  ## 2. Pin the right repos                                                                                                                                   
                                                                                                                                                              
  In the sidebar you can see `spec`, `agentcontract-action`, `agentcontract-rs` listed but not pinned/ordered. Go to **Settings → Member privileges** is not  
  what you need — on the org Overview page click **"Pin repositories"** (visible when logged in as owner) and pin in this order:
                                                                                                                                                              
  1. `spec` — the anchor                                                                                                                                      
  2. `agentcontract-py` — most accessible, pip install
  3. `agentcontract-action` — CI/CD, Marketplace                                                                                                              
  4. `agentcontract-ts`                                                                                                                                       
  5. `agentcontract-rs`                                                                                                                                       
  6. `contracts`                                                                                                                                              
                                                                                                                                                              
  ---                                                       

  ## 3. Add org description and URL                                                                                                                           
   
  Go to **Settings** (org) → fill in:                                                                                                                         
  - **Description:** `Open spec for behavioral contracts on AI agents — ESLint for AI`
  - **URL:** `https://llmops.pro` (or the spec repo URL)                                                                                                      
  - **Email:** Mauro's contact                                                                                                                                
                                                                                                                                                              
  ---      
