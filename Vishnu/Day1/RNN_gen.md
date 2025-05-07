┌────────────────────────────┐
│ 1. Configuration & Setup   │
├────────────────────────────┤
│ Set hyperparameters        │
│ Set random seed & device   │
└────────────────────────────┘
           ↓
┌────────────────────────────┐
│ 2. Data Preparation        │
├────────────────────────────┤
│ - Load text corpus         │
│ - Create vocab (char2idx)  │
│ - Encode input text        │
│ - Split into sequences     │
│ - Define PyTorch Dataset   │
└────────────────────────────┘
           ↓
┌────────────────────────────┐
│ 3. Model Definition        │
├────────────────────────────┤
│ - nn.Embedding layer       │
│ - nn.RNN layer (multi-layer)│
│ - nn.Linear output layer   │
└────────────────────────────┘
           ↓
┌────────────────────────────┐
│ 4. Training Loop           │
├────────────────────────────┤
│ For each epoch:            │
│  - Iterate over batches    │
│  - Forward pass            │
│  - Compute loss            │
│  - Backward pass           │
│  - Gradient clipping       │
│  - Optimizer step          │
└────────────────────────────┘
           ↓
┌────────────────────────────┐
│ 5. Text Generation         │
├────────────────────────────┤
│ - Provide seed text        │
│ - Use trained RNN to       │
│   generate new characters  │
└────────────────────────────┘
