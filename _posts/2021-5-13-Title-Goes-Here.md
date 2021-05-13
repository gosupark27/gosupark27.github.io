## Nice Hook bruh

## Today's Tasks
1. Finishing up on Clojure Koans 

## Challenges 

## TIL 
- The difference between `vars` and `refs`. 
  - `vars` ensure safe use of mutable storage locations via *thread isolation*
  - `refs` ensure safe **shared** use of mutable storage locations via STM (software transactional memory)
    -  *This is where the concept of **transaction** comes into play*
    -  Also, Clojure transactions are like database transactions - they ensure that *all* actions on Refs are **atomic**, **consistent** & **isolated**. 
        - <ins>Atomic:</ins>  Every change to Refs made within a transaction occurs or none do.
        - <ins>Consistent:</ins>  Each new value can be checked with a validator function before allowing the transaction to commit.
        - <ins>Isolated:</ins>  No transaction sees the effects of any other transaction while it is running.
    -  Refs are bound to a single storage location for their lifetime
    -  Refs only allow mutation of that location to occur **within a transaction**

## Looking Ahead To TGIF 
