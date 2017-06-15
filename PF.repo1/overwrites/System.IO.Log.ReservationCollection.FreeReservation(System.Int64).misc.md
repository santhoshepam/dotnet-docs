---
uid: System.IO.Log.ReservationCollection.FreeReservation(System.Int64)
additional_notes.overrides: *content
---

<p>When you inherit from <xref href="System.IO.Log.ReservationCollection"></xref>, you must implement this method to actually release space in the record sequence. You should not call <xref href="System.IO.Log.ReservationCollection.ReservationFreed(System.Int64)"></xref> when this method is complete; that logic is handled for you.  
  
 When you free records, you must free the same records that you reserved together in a previous call to the <xref href="System.IO.Log.IRecordSequence.ReserveAndAppend*"></xref> method.</p>


