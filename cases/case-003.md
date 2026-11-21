# Turning uneven behaviour into an engineering requirement

**Context.** An agent behaved unevenly around a platform update. The lab could observe the change in behaviour and had too little information to diagnose its cause.

**Oleksandra's contribution.** She wrote a requirement for the future local system. The owner should be able to approve or defer updates, inspect installed versions and configuration, compare a suspect state with a known-good state, and roll back when technically supported. She also called for a small, repeatable behavioural comparison to help investigate regressions. An agent recorded her requirement in the lab's working specification.

**Result.** The lab gained an explicit requirement and a way to assess it in a future deployment. The cause of the original behaviour remains unknown. Implementation and testing of the local system were still ahead at the time of the snapshot.

**Draft acceptance check.** Given a known-good baseline and a later update, the owner can identify what changed, verify the deployment state, compare behaviour against the baseline and restore the previous state where supported.
