# Inflexible Requirement #1
    - Zero coupling between child projects
        - No import of functions/objects/classes/etc
        - No shared state
        - Shared libs through ModelFederation is ok

# Inflexible Requirement #2
    - Near-zero coupling between container and child apps
        - Container shouldn't assume that a child is using a particular framework
        - Any necessary communication done with callbacks or simple events

# Inflexible Requirement #3
    - CSS from one project shouldn't affect another

# Inflexible Requirement #4
    - Version control shouldn't have any impact on the overall project
        - some people want to use monorepos
        - some people want to use separate repos

# Inflexible Requirement #5
    - Container should be able to decide a specific version of the module
        - Container will always use the latest version of a child app (no redeploy)
        - Container can specify exactly what version of a child it wants to use (redeploy)

# Deployment
