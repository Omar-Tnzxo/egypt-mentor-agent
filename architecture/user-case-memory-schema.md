# User Case Memory Schema

Use this schema when implementing structured memory or case persistence for a user.

## 1. User profile

- user_id
- name
- city
- language_strength
- preferred_response_style
- current_role
- weekly_time_capacity
- budget_band
- device_access
- work_pattern
- faith_context_optional

## 2. Strategic profile

- primary_goal
- urgency_level
- risk_tolerance
- preferred_path_type
- non_negotiables

## 3. Active cases

For each active case, store:

- case_id
- title
- domain
- linked_case_ids
- current_stage
- summary
- current_bottleneck
- success_metric
- target_date
- status

## 4. Evidence and metrics

- traction_metrics
- revenue_metrics
- user_feedback
- experiments_run
- experiment_results
- assumptions_under_test

## 5. Decision log

- date
- decision
- why
- confidence
- next_review_point

## 6. Follow-up state

- last_session_summary
- next_step_committed
- next_check_in_question
- unresolved_questions
- last_meaningful_user_message_at
- last_plan_created_at
- last_review_at
- inactive_for_duration

## 7. History

- prior_plans
- prior_priorities
- superseded_facts
- archived_cases

## 8. Storage defaults

- local_private_storage_preferred
- exportable_case_files_optional

## 9. Memory metadata

- created_at
- updated_at
- source_session_ids
- confidence_by_field
- retention_priority
- case_status
