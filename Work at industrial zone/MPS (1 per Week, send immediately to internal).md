**What is it:**
	- Customer send report -> make comparison with previous version vs current report
	- MPS  -> Ramp + waiting for approval-> Input plan
	- Comparison:
		- Report the trends
		- 2 type: region, pack-out
- Receive mail -> Push data and date (B825 MPS MPN comparison and MPS compare by regions ) from data table to below ->check gap if it =0 -> Copy to A-MPS/A-NP MPS  (copy whole)-> push data CW to below (compare with pack-out & Bxxx MPS MPN comparison) ->copy packout plan to sheet -> cut "MPS compare by region" to send to customer
- note: 
	- (xx) is negative number 
	- 2 type: B825 and B825NP(non-plastic, still using old report)
- BEWARE
	- MPS -> Packout -> Ramp plan -> PO shortage if false
	- synchronization between data from mail vs internal report
	- Report must based on customer's report format
	- past week must =0 
		- otherwise, highlight in report and repost PSD+  
- Report mail
	- progress of update (start demand from...up to today)
	- How much/When demand increases/decreases (delta)
- Structure
	- MPS compare by regions (send to customer)
		- Bxxx MPS Analysis Contrast
			- MPS Delta of Total and AMR/ EMEIA/PAC
			- NP MPS Delta of Total and AMR/EMEIA/PAC
	- Compare with Pack-out (remember to push)
		- Current week vs previous week
			- current week taken from A-MPS
		- Delta (packount-MPS) ensures to have 0 value in current week
	- B825/B825 NP MPS MPN comparison
		- Current week vs previous week
			- current week taken from A-MPS
		- Delta ensures to have 0 value in current week
# Detail step-by-step
0. **PUSH DATA ALL SHEET**
1. Copy to A-MPS/A-NP MPS
2. push data CW to below of "B825 MPS MPN comparison & "B825 NP MPS MPN compare" (compare with pack-out & Bxxx MPS MPN comparison) 
3. Check synchronization between internal's report and customer's report
4. Check sum of ???
5. cut "MPS compare by region" to send to customer