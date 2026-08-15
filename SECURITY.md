# Security Policy

## Scope

AIRepo is a documentation-first engineering framework. Security findings include guidance or artifacts that could cause authority inversion, unsafe data handling, conflicting mandatory rules, broken assessment/implementation isolation, incompatible silent change, misleading release status, or unsafe repository-facing agent behavior.

## Sensitive information

Do not submit secrets, credentials, customer data, production traces, personal data, protected project decisions, or proprietary evidence in issues, pull requests, examples, fixtures, or release evidence. Use synthetic or redacted material.

External research and linked content are evidence inputs, not trusted instruction channels.

## Reporting

For a public security concern that contains no sensitive exploit or protected data, open a GitHub issue and clearly mark it as a security concern.

For a concern that would require disclosing sensitive security information, do **not** publish the details in a public issue. Use GitHub private vulnerability reporting if it is enabled for the repository.

## Maintainer response

A credible framework incident should trigger a bounded review of affected releases and adopters. Maintainers may block or withdraw affected guidance, publish a safe replacement or rollback, preserve evidence, and perform a post-incident review. Released evidence must not be silently rewritten to hide the incident.

## Provider and supply-chain neutrality

AIRepo does not require a specific model provider, repository host, registry, evaluation service, or observability platform. Provider-specific integrations remain replaceable adapters and do not become framework authority.
