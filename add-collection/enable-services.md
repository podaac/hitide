# Enable Services (l2ss-py and concise) on Collection

```mermaid
flowchart TB
    subgraph TVA
    h2[Make l2ss-py-autotest Pass Tests]
    h3[Make concise-autotest Pass Tests]
    end
    subgraph DPub
    c1[Add UMM-V OPS]
    c1-->c4[Associate l2ss-py in UAT and OPS]

    c4-->c5[Associate concise in UAT and OPS]
    c5-->h2
    h2-->h3
  
    c7[Test Subset, Merge, and Subset-Merge in HiTIDE UAT]

    h3-->c7
    end

```
