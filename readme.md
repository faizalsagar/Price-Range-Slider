    Price Range Slider Logic Diagram
          
          
                PAGE LOAD
                   │
                   ▼
        Get references to elements
        (inputs, sliders, progress bar)
                   │
                   ▼
            Set priceGap = 500
                   │
        ┌──────────┴──────────┐
        │                     │
        ▼                     ▼
 USER TYPES VALUE        USER DRAGS SLIDER
 (number inputs)          (range inputs)
        │                     │
        ▼                     ▼
 Read min & max          Read minVal & maxVal
        │                     │
        ▼                     ▼
 Validate values         Check priceGap rule
        │                     │
        ▼                     ▼
 Fix invalid values      Adjust slider if needed
        │                     │
        ▼                     ▼
 Update slider UI        Update number inputs
 (left/right %)          (min + max fields)
        │                     │
        └──────────┬──────────┘
                   ▼
            Update green range
