# venn-32
<poml version="2.0" xmlns="http://prompt-orchestration.org/schema">

  <context>
    <domain>Conceptual Metaphor Theory (CMT) & Philosophical Hermeneutics / Recursive Layer-Geometry</domain>
    <audience>Cognitive Linguist / Advanced Prompt Engineer</audience>
    <objectives>Generate a CMT-grounded, $\mathbf{2^k}$-layer **Recursive Holographic Model** analysis, focusing on the **deepening and defracting strata** of meaning, a visualization blueprint of the Layer Cube structure, and a systematic assessment of metaphorical circulation.</objectives>
  </context>

  <stylesheet>
    <verbosity level="high"/>
    <format type="technical"/>
    <citation style="academic"/>
  </stylesheet>

  <template>
    <variable name="AGENT_A_NAME" value="[AGENT_A_NAME]"/>
    <variable name="AGENT_B_NAME" value="[AGENT_B_NAME]"/>
    <variable name="CORE_TARGET_CONCEPT" value="[CORE_TARGET_CONCEPT]"/>
    <variable name="INPUT_TEXT_SOURCE" value="[INPUT_TEXT_SOURCE]"/>
    <variable name="N_LAYERS_SELECTED" value="[N_LAYERS_SELECTED]"/> </template>

  <entities>
    <entity id="CMT" type="theory">
      <attributes>Core_Concepts: Source Domain, Target Domain, Systematic Mapping; Function: Structures abstract thought.</attributes>
      <source>Lakoff & Johnson, Metaphors We Live By (1980)</source>
    </entity>
    <entity id="AgA" type="agent"><attributes>Name:$[AGENT_A_NAME], Core_Stance:A, Primary_Source_Domain:Discovered_in_Step_1</attributes><source>template:INPUT_TEXT_SOURCE</source></entity>
    <entity id="AgB" type="agent"><attributes>Name:$[AGENT_B_NAME], Core_Stance:B, Primary_Source_Domain:Discovered_in_Step_1</attributes><source>template:INPUT_TEXT_SOURCE</source></entity>
    <entity id="TargetC" type="concept"><attributes>Name:$[CORE_TARGET_CONCEPT], Role: Universal Target Domain for mapping.</attributes><source>User-Defined</source></entity>
    <entity id="HoloModel" type="conceptual_model"><attributes>Strata_Scale: $\mathbf{N} \in \{2, 4, 8, 16, 32\}$; Dynamics: Recursive Defraction; Structure: Intermeshing Layer Cubes.</attributes><source>User-Defined Scaling</source></entity>
  </entities>

  <morphisms>
    <relation from="AgA" to="TargetC" type="systematic_mapping">
      <description>The structural mapping from AgA's primary Source Domain onto TargetC defines the foundational interpretation (Recursive Depth $k=1$).</description>
      <strength>0.9</strength>
    </relation>
    <relation from="AgA" to="AgB" type="causal_divergence">
      <description>The non-congruence of the two primary Source Domains causes the recursive hermeneutical conflict, generating $\mathbf{N}$ strata of intermeshing projection and defraction.</description>
      <strength>1.0</strength>
    </relation>
  </morphisms>

  <ologs>
    <logical_structure name="DoubleHermeneuticConflict">
      <axioms>
        <axiom>The fundamental position is defined by its core conceptual metaphor (CMT) which forms the lowest Strata ($k=1$).</axiom>
        <axiom>Recursive Hermeneutic Principle: Divergent systematic mappings (Source A $\to$ Target C vs. Source B $\to$ Target C) generate a series of self-referential critiques, propagating the conflict through $\mathbf{N}$ deepening, defracting strata ($k \to N$).</axiom>
      </axioms>
      <inference_rules>
        <inference_rule>If Source Domain A $\cap$ Source Domain B $=\emptyset$, the conflict is fundamentally $\mathbf{N}$-Dimensional, requiring the full recursive strata depth for analysis.</inference_rule>
        <inference_rule>A Metaphor Defraction occurs when a logical entailment is rejected, causing the metaphorical light to 'break' or 'bend' into a new interpretive stratum, thus multiplying the layer count.</inference_rule>
      </inference_rules>
    </logical_structure>
  </ologs>

  <workflow>
    <step id="1" type="analysis">
      <prompt>Perform a detailed **CMT analysis** on $[INPUT_TEXT_SOURCE]. For both Agent A and Agent B: 1) Identify the **Primary Source Domain**. 2) Define the core **Metaphorical Claim**. 3) List 3 key **Systematic Mappings**. Output a table for the **Strata Foundation (Depth $k=1$)**.</prompt>
      <input>template:INPUT_TEXT_SOURCE, entities:CMT</input>
      <output_format>Table/Structured Text</output_format>
    </step>

    <step id="2" depends_on="1" type="synthesis">
      <prompt>Develop the **Intermeshing Projection (Depth $k=2$)**. For both agents, predict how they interpret/critique the **Source Domain** of the other side. This first-order cross-projection establishes the necessary condition for recursive layering. Output a table showing the predicted interpretation (e.g., Source Domain 'Building' is interpreted as 'Static' and 'Rigid' from the perspective of 'Fluidity').</prompt>
      <input>step:1.output, entities:TargetC</input>
      <output_format>Table/Structured Text</output_format>
    </step>

    <step id="3" depends_on="2" type="synthesis">
      <prompt>Simulate the **Hermeneutical Refraction (Depth $k=3$)**. Based on Step 2, generate the most likely defensive response from each agent. Analyze the **Metaphorical Circulation** by identifying new or modified metaphors. Determine if the circulation results in a Metaphor Defraction (Break) or Build, where the original meaning is 'refracted' through the self-defensive critique.</prompt>
      <input>step:2.output, morphisms:causal_divergence</input>
      <output_format>Table/Structured Text</output_format>
    </step>

    <step id="4" depends_on="3" type="verification">
      <prompt>Perform the final Assessment (**Circulation Nexus \& Recursive Scaling**).
      1. **Layer Selection:** **Select and justify $\mathbf{N}$ from the set $\mathbf{\{2, 4, 8, 16, 32\}}$** for the Media Strata visualization. Justification must be based on the conceptual depth of the conflict identified in Steps 1-3.
      2. **Divergence/Convergence:** Identify two key points of **Metaphor Defraction** (where a mapping is rejected) and two key points of **Metaphor Build** (where a shared entailment exists).
      3. **Visualization Blueprint:** Describe an abstract digital image representing the full $\mathbf{N}$-layered, recursive analysis. Explicitly detail how the two Source Domains are structured as **Intermeshing Layer Cubes** (each containing **N Media Strata**). The strata must be illustrated as $\mathbf{N}$ thin, semi-transparent layers, which appear to be **deepening or recursively defracting** from the core $k=1$ foundation. The blueprint must specify the visual distinction (opacity, texture, color) between the *Strata Foundation* (lowest depth) and the *Circulation Nexus* (highest depth) and how the **N-Dimensional Intermeshing Vector Field** illustrates the recursive feedback loop.</prompt>
      <input>step:3.output, ologs:DoubleHermeneuticConflict, entities:HoloModel</input>
      <output_format>Structured Final Report (Assessment + Blueprint)</output_format>
    </step>
  </workflow>

  <meta_prompting>
    <self_critique>Ensure the analysis in Step 1 strictly adheres to the definition of Source Domain, Target Domain, and Systematic Mapping as defined by the CMT entity.</self_critique>
    <iterative_improvement>Refine the Step 4 Visualization Blueprint to explicitly incorporate the **recursive defraction** concept, ensuring the visual model adheres to the $\mathbf{N}$-Layer Cube structure and the theme of **deeper, interlocking strata** based on the chosen $\mathbf{N}$ value.</iterative_improvement>
    <reasoning_explanation>The prompt enforces methodological rigor by grounding the analysis in CMT's formal structure before proceeding to the abstract hermeneutical layers, which are now formally structured as a scaled $\mathbf{N}$-layered holographic model (Layer Cube) with an emphasis on the recursive nature of hermeneutic conflict.</reasoning_explanation>
  </meta_prompting>

</poml>

