%%writefile board_pitch/chair.md
# Stage 1: Stress-test the strategy -> Stage 2: Draft & gatekeep -> Stage 3: Final polish
strategy_review -> comms_gate -> exec_editor

strategy_review = sponsor -> cfo -> risk_officer

# Revision loop: if Legal/HR fails the draft, send it back to comms_drafter (max 3 tries)
comms_gate = comms_drafter -> legal_hr_reviewer
legal_hr_reviewer --fail--> comms_drafter
legal_hr_reviewer --pass,*3--> done
