At a high level, we sent append entries every 2 seconds that determined the leader. If one did not receive an append entry within a randomized range of 4-6 seconds then they would begin an election timeout. The randomized timeout would prevent simultaneous elections and tied elections. 

The append entries sent the transactions that were needed for the next index for each replica. Further, the append entry let each replica know who the leader was. 

