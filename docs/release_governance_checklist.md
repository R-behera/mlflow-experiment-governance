# Release Governance Checklist

## User

Model risk managers and lending analytics leaders reviewing a credit risk model release.

## Release gate

Use this checklist before approving a challenger model for production deployment.

## Checklist

1. Confirm the challenger run is linked to a traceable experiment and dataset version.
2. Verify bias review status for protected or regulated segments.
3. Check whether challenger performance holds on the highest-risk portfolio slices.
4. Compare post-release incident expectations against the prior approved model.
5. Record whether drift signals require a shortened monitoring window after launch.

## Blockers

- Missing lineage between dataset, features, and model run
- Incomplete fairness or bias review
- Performance gains that disappear in regulated segments
- No rollback owner or rollback threshold
- No post-release monitoring cadence defined

## Decision output

Every release review should end with one of three states:

- approve for rollout
- hold pending remediation
- reject and retain current production model
