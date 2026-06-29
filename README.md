# Minor-Project-1
Here is a highly professional, well-structured, and attractive README.md description for your GitHub repository. It acts as the face of your project, making it easy for recruiters and open-source contributors to understand your engineering decisions at a glance.# GroupDNA: WhatsApp Group Chat, Decoded 🧬"Spotify Wrapped, but for your friend group."GroupDNA is a lightweight, dependency-conscious Python engine designed to parse, analyze, and decode raw WhatsApp group chat export logs. By converting unstructured textual data streams into distinct analytical metrics, GroupDNA maps out behavioral patterns, message velocities, and communication velocities to build a data-driven social fingerprint of any friend group.  The pipeline relies on native Python structures and NumPy matrix manipulations rather than heavy data science frameworks, showcasing optimized string parsing and lightweight data processing.  
🚀 Features1. High-Fidelity Chat ParserDeterministic Logging: Gracefully processes multi-line text blocks, strips tracking system alerts, and isolates structural variables like timestamps, senders, and content strings.  System Event Filtering: Explicitly accounts for and isolates media attachments (<Media omitted>) and deleted message headers to maintain statistical integrity. 
2. Matrix-Based Activity HeatmapsNumPy Acceleration: Maps hourly messaging velocity per participant using a 24-hour frequency matrix.  Console Visualization: Renders space-optimized ASCII density blocks directly to the console to visually track night owls versus early birds. 
3. Response Velocity & Chronological Silence TrackingSequential Delta Analysis: Computes conversational handoffs between different users, calculating response speeds down to the minute.  Calendar Timeline Mapping: Generates a synthetic chronological timeline matching the chat duration to evaluate absolute consecutive days of zero user interaction (Longest Silent Streaks). 
4. Linguistic Archetype ProfilingImplements an algorithmic scoring system that evaluates individual text volumes, word lengths, capitalization frequencies, and curated lexicons to assign exclusive behavioral personas:  📢 THE SPAMMER: Characterized by high transmission bursts.  📖 THE STORYTELLER: Assigned via high average word counts per message.  👑 THE DRAMA QUEEN: Triggered by specific upper-case token weightings.  🧸 THE GROUP MOM: Identified through linguistic match-keys like safety reminders and caring lexicons.  👻 THE GHOST: Triggered by zero-activity matrix spans and high sequential silent streaks. 
📊 Analytics Dashboard SnapshotWhen running Lavanya_Sawant_Project_1.ipynb on sample logs (such as the included 60-day, 3,100+ message sample from a Hostel Bois 4ever chat), the pipeline renders a neat console visualization: 
=======================================================
                  *THE CHAT PARSER* 
=======================================================
Successfully parsed 3174 messages from 6 participants.
Skipped 4 system messages.

=======================================================
                 *MESSAGES PER PERSON*
=======================================================
Rahul      :  953 (30.0%) -> THE SPAMMER
Priya      :  718 (22.6%) -> THE GROUP MOM
Neha       :  635 (20.0%) -> THE DRAMA QUEEN
Aman       :  490 (15.4%) -> THE GROUP MOM
Karan      :  354 (11.2%) -> THE STORYTELLER
Vikas      :   24 (0.8%)  -> THE GHOST

Busiest day      : 04/05/24 (76 messages)
Busiest hour     : 18:00 (248 total messages)

=========================================================
           *ACTIVITY HEATMAP (messages by hour)*
=========================================================
            00 03 06 09 12 15 18 21
Rahul        .  .  .  .  ▒  ▒  █  █ 
Priya        .  .  .  █  █  ░  ▒  ░ 
Vikas        .  .  .  ░  ▒  ░  ▒  ░ 

=======================================================
             *THIS GROUP'S FAVOURITE WORDS*
=======================================================
guys          318  ███████████████
today         257  ████████████
everyone      187  ████████

🛠️ Technical BreakdownCore Language: Python 3  
Primary Paradigm: Functional logic & rule-based scoring models 
Key Libraries: NumPy (Heatmap grid accumulation),
datetime (Timestamp and timedelta operations)  
Development Notebook: Lavanya_Sawant_Project_1.ipynb
