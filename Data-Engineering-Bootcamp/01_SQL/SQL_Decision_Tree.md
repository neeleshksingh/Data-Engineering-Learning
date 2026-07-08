Read Question
        │
        ▼
Need data from another table?
        │
   Yes ─────► JOIN
        │
       No
        │
        ▼
Need fewer rows?
        │
   Yes ─────► GROUP BY
        │
       No
        │
        ▼
Need same rows + extra info?
        │
   Yes ─────► WINDOW FUNCTION
        │
       No
        │
        ▼
Need Top/First/Last?
        │
   Yes ─────► ROW_NUMBER / RANK / DENSE_RANK