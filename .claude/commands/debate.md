For a given query ($ARGUMENTS):

1. Create a folder structure for this debate:
   - Create a `debates` folder if it doesn't exist
   - Create a subfolder with format `debates/YYYY-MM-DD-topic-slug` (e.g., `debates/2025-01-29-healthcare-reform`)
   - Initialize empty files: `transcript.md` and `summary.md`

2. Have the moderator sub agent come up with a plan to host a debate between the democrat and the republican sub agent. The truth seeker sub agent is observing.

3. Have the moderator ask the first question to either the republican or democrat sub agent.

4. Instruct both the democrat and republican agents to:
   - Use the WebSearch tool to find current data and statistics
   - Include citations with URLs in their responses
   - Reference specific sources like think tanks, government reports, and academic studies

5. Have the debate continue for at least 3 turns until the truth seeking agent has a firm perspective.

6. Throughout the debate, append each exchange to the `transcript.md` file with proper formatting:
   - Include timestamps, speaker names, and full responses
   - Preserve all citations and links
   - Format with clear section headers for each round

7. Have the truth seeking agent make a decision on its stance on the issue and explain why.

8. Generate a comprehensive one-page summary by the truth-seeking agent and save it to `summary.md`:
   - Executive summary of key arguments from both sides
   - Evidence assessment with citations
   - Final position with supporting data
   - Actionable policy recommendations

9. Update `transcript.md` with the complete debate including the truth-seeker's final assessment.