---
uid: System.IO.Log.ReservationCollection.MakeReservation(System.Int64)
additional_notes.overrides: *content
---

<p>When you inherit from <xref href="System.IO.Log.ReservationCollection"></xref>, you must implement this method to actually reserve space in the record sequence. You should not call <xref href="System.IO.Log.ReservationCollection.ReservationMade(System.Int64)"></xref> when this method is complete; that logic is handled for you.</p>


