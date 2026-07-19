### G3_A0_DECISION.json

  {
    "decision": "NO_DECISION_INSUFFICIENT_EVIDENCE",
    "evaluated_at": "2026-07-19T03:34:22.316576+00:00",
    "gate": "G3_METHOD_GATE",
    "phase1_completion": {
      "completed_outer_folds": [
        0,
        1,
        2,
        3,
        4
      ],
      "frozen_code_sha256_across_folds": true,
      "methods": [
        "B1",
        "Mask R-CNN",
        "B3",
        "detector_score",
        "sam_predicted_iou",
        "sam_stability",
        "jitter_variance",
        "area_component_rule",
        "lightweight_quality_regressor",
        "B5"
      ],
      "outer_folds": [
        0,
        1,
        2,
        3,
        4
      ],
      "outer_test_evaluations_per_patient": 1,
      "outer_test_used_for_route_or_threshold_selection": false,
      "pointrend_executed": false,
      "seed": 2027
    },
    "phase1_report": {
      "artifact_and_leakage_audit": {
        "color_artifact_dependency": false,
        "label_leakage": false,
        "status": "NOT_ESTIMABLE_DUE_TO_INSUFFICIENT_PHASE1_EVIDENCE",
        "text_artifact_dependency": false
      },
      "b3_vs_mask_rcnn": {
        "delta_definition": "B3 patient-macro Dice minus Mask R-CNN patient-macro Dice",
        "dice_delta_ci_high": 1.0,
        "dice_delta_ci_low": -1.0,
        "efficiency_measured": false,
        "status": "NOT_ESTIMABLE_DUE_TO_INSUFFICIENT_PHASE1_EVIDENCE"
      },
      "b5_vs_strongest_simple_control": {
        "absolute_negative_view_action_rate_reduction": 0.0,
        "all_controls_same_full_cohort_evaluator": true,
        "automatic_coverage": 0.0,
        "lesion_recall_delta_ci_low": -1.0,
        "overall_referral_rate": 1.0,
        "patient_macro_dice_delta_ci_low": -1.0,
        "positive_refer_counted_as_failure": true,
        "status": "NOT_ESTIMABLE_DUE_TO_INSUFFICIENT_PHASE1_EVIDENCE"
      },
      "candidate_pool_oracle_at_98pct_lesion_sensitivity": {
        "lesion_sensitivity": 0.98,
        "negative_view_fp_reduction_attainable": false,
        "status": "NOT_ESTIMABLE_DUE_TO_INSUFFICIENT_PHASE1_EVIDENCE"
      },
      "event_sufficiency": {
        "any_meta_fold_single_class": false,
        "confidence_intervals_stably_estimable": false,
        "fold_failures": [
          {
            "any_meta_fold_single_class": false,
            "effective_failure_events_sufficient": false,
            "reason": "UNSTABLE_THRESHOLD / NO_DECISION: lightweight_quality_regressor: {'status': 'UNSTABLE_THRESHOLD /
            NO_DECISION', 'threshold': 0.005818983800356026, 'fold_thresholds': [{'heldout_meta_fold': 0, 'threshold':
            0.005818983800356026, 'training_fold_sensitivity': 0.9722222222222222, 'target_attainable': False}, {'heldout_meta_fold':
            1, 'threshold': 0.005818983800356026, 'training_fold_sensitivity': 0.972972972972973, 'target_attainable': False},
            {'heldout_meta_fold': 2, 'threshold': 0.005818983800356026, 'training_fold_sensitivity': 0.9622641509433962,
            'target_attainable': False}, {'heldout_meta_fold': 3, 'threshold': 0.3016642407532461, 'training_fold_sensitivity':
            0.9821428571428571, 'target_attainable': True}], 'fold_threshold_range': 0.2958452569528901, 'max_fold_threshold_range':
            0.25, 'oof_lesion_sensitivity': 0.9764705882352941, 'oof_patient_macro_normal_fp_rate': 0.8342394873644873,
            'target_attainable': False, 'selection_source': 'leave_one_meta_fold_out_then_median_inner_meta_oof_only'}",
            "status": "NO_DECISION_INSUFFICIENT_EVIDENCE_PENDING_COMPLETE_FIVE_FOLDS",
            "threshold_unstable": true
          },
          {
            "any_meta_fold_single_class": false,
            "effective_failure_events_sufficient": false,
            "reason": "UNSTABLE_THRESHOLD / NO_DECISION: lightweight_quality_regressor: {'status': 'UNSTABLE_THRESHOLD /
            NO_DECISION', 'threshold': 0.21075371050969569, 'fold_thresholds': [{'heldout_meta_fold': 0, 'threshold':
            0.14537104498263126, 'training_fold_sensitivity': 0.9859154929577465, 'target_attainable': True}, {'heldout_meta_fold':
            1, 'threshold': 0.14537104498263126, 'training_fold_sensitivity': 0.9848484848484849, 'target_attainable': True},
            {'heldout_meta_fold': 2, 'threshold': 0.41411142494413244, 'training_fold_sensitivity': 0.9852941176470589,
            'target_attainable': True}, {'heldout_meta_fold': 3, 'threshold': 0.2761363760367601, 'training_fold_sensitivity':
            0.9838709677419355, 'target_attainable': True}], 'fold_threshold_range': 0.2687403799615012, 'max_fold_threshold_range':
            0.25, 'oof_lesion_sensitivity': 0.9775280898876404, 'oof_patient_macro_normal_fp_rate': 0.6286546786546786,
            'target_attainable': False, 'selection_source': 'leave_one_meta_fold_out_then_median_inner_meta_oof_only'}",
            "status": "NO_DECISION_INSUFFICIENT_EVIDENCE_PENDING_COMPLETE_FIVE_FOLDS",
            "threshold_unstable": true
          },
          {
            "any_meta_fold_single_class": false,
            "effective_failure_events_sufficient": false,
            "reason": "UNSTABLE_THRESHOLD / NO_DECISION: area_component_rule: {'status': 'UNSTABLE_THRESHOLD / NO_DECISION',
            'threshold': 0.38394535363088067, 'fold_thresholds': [{'heldout_meta_fold': 0, 'threshold': 0.4756303111058337,
            'training_fold_sensitivity': 0.9857142857142858, 'target_attainable': True}, {'heldout_meta_fold': 1, 'threshold':
            0.2922603961559277, 'training_fold_sensitivity': 0.984375, 'target_attainable': True}, {'heldout_meta_fold': 2,
            'threshold': 0.2922603961559277, 'training_fold_sensitivity': 0.9866666666666667, 'target_attainable': True},
            {'heldout_meta_fold': 3, 'threshold': 0.6557262142862044, 'training_fold_sensitivity': 0.9827586206896551,
            'target_attainable': True}], 'fold_threshold_range': 0.3634658181302767, 'max_fold_threshold_range': 0.25,
            'oof_lesion_sensitivity': 0.9775280898876404, 'oof_patient_macro_normal_fp_rate': 0.5903101528101528,
            'target_attainable': False, 'selection_source': 'leave_one_meta_fold_out_then_median_inner_meta_oof_only'}",
            "status": "NO_DECISION_INSUFFICIENT_EVIDENCE_PENDING_COMPLETE_FIVE_FOLDS",
            "threshold_unstable": true
          },
          {
            "any_meta_fold_single_class": false,
            "effective_failure_events_sufficient": false,
            "reason": "UNSTABLE_THRESHOLD / NO_DECISION: lightweight_quality_regressor: {'status': 'UNSTABLE_THRESHOLD /
            NO_DECISION', 'threshold': 0.16305705159157358, 'fold_thresholds': [{'heldout_meta_fold': 0, 'threshold':
            0.16305705159157358, 'training_fold_sensitivity': 0.9830508474576272, 'target_attainable': True}, {'heldout_meta_fold':
            1, 'threshold': 0.6023991711245025, 'training_fold_sensitivity': 0.9855072463768116, 'target_attainable': True},
            {'heldout_meta_fold': 2, 'threshold': 0.16305705159157358, 'training_fold_sensitivity': 0.9846153846153847,
            'target_attainable': True}, {'heldout_meta_fold': 3, 'threshold': 0.16305705159157358, 'training_fold_sensitivity':
            0.9859154929577465, 'target_attainable': True}], 'fold_threshold_range': 0.4393421195329289, 'max_fold_threshold_range':
            0.25, 'oof_lesion_sensitivity': 0.9886363636363636, 'oof_patient_macro_normal_fp_rate': 0.5917330447330447,
            'target_attainable': True, 'selection_source': 'leave_one_meta_fold_out_then_median_inner_meta_oof_only'}",
            "status": "NO_DECISION_INSUFFICIENT_EVIDENCE_PENDING_COMPLETE_FIVE_FOLDS",
            "threshold_unstable": true
          }
        ],
        "max_fold_threshold_range": 1.0,
        "meta_fold_unique_patient_counts": {},
        "unique_patient_counts": {}
      },
      "phase1_completion": {
        "completed_outer_folds": [
          0,
          1,
          2,
          3,
          4
        ],
        "frozen_code_sha256_across_folds": true,
        "methods": [
          "B1",
          "Mask R-CNN",
          "B3",
          "detector_score",
          "sam_predicted_iou",
          "sam_stability",
          "jitter_variance",
          "area_component_rule",
          "lightweight_quality_regressor",
          "B5"
        ],
        "outer_folds": [
          0,
          1,
          2,
          3,
          4
        ],
        "outer_test_evaluations_per_patient": 1,
        "outer_test_used_for_route_or_threshold_selection": false,
        "pointrend_executed": false,
        "seed": 2027
      },
      "predicted_box_localization": {
        "metric": "patient_cluster_bootstrap_recall_at_1_fp_per_view",
        "recall_ci_high": 1.0,
        "recall_ci_low": 0.0,
        "status": "NOT_ESTIMABLE_DUE_TO_INSUFFICIENT_PHASE1_EVIDENCE"
      },
      "protocol_version": "2.3",
      "schema_version": 3,
      "simple_control_inner_meta_oof_ranking": {
        "controls": [
          "detector_score",
          "sam_predicted_iou",
          "sam_stability",
          "jitter_variance",
          "area_component_rule",
          "lightweight_quality_regressor"
        ],
        "selection_score_source": "PATIENT_GROUPED_META_OOF_ONLY",
        "status": "NOT_ESTIMABLE_DUE_TO_INSUFFICIENT_PHASE1_EVIDENCE",
        "strongest_control": "detector_score"
      }
    },
    "phase2_authorized": false,
    "point_rend_phase1": "FORBIDDEN_NOT_RUN",
    "protocol_version": "2.3",
    "provenance": {
      "code_tree_sha256": "47faa8eeaac7fe279efd08711586dce150f0b7ea795ca50ebeda01ce6d5c6323",
      "config_sha256": "2d2bb53931cb84f047ec655354bbe9f402825f4209dc168fe45d89a52fe45cd8",
      "inner_meta_only_selection": true,
      "manifest_sha256": "e13673f9e116c3e56cef194e4071ce5022c7930437f240225472913b2e86f5f6",
      "outer_test_interim_selection": false,
      "phase1_report_path": "/workspace/ScreenBUS/server_bundle/runtime/output/phase1/PHASE1_FIVE_FOLD_REPORT.json",
      "phase1_report_sha256": "bf018bb336308058e928552ec9dc8be06ae2b9001ce5ffd00351f0fd824bd7be"
    },
    "schema_version": 3,
    "status": "G3_RECOMPUTED_FROM_COMPLETE_PHASE1"
  }

  ### PHASE1_FIVE_FOLD_REPORT.json

  {
    "artifact_and_leakage_audit": {
      "color_artifact_dependency": false,
      "label_leakage": false,
      "status": "NOT_ESTIMABLE_DUE_TO_INSUFFICIENT_PHASE1_EVIDENCE",
      "text_artifact_dependency": false
    },
    "b3_vs_mask_rcnn": {
      "delta_definition": "B3 patient-macro Dice minus Mask R-CNN patient-macro Dice",
      "dice_delta_ci_high": 1.0,
      "dice_delta_ci_low": -1.0,
      "efficiency_measured": false,
      "status": "NOT_ESTIMABLE_DUE_TO_INSUFFICIENT_PHASE1_EVIDENCE"
    },
    "b5_vs_strongest_simple_control": {
      "absolute_negative_view_action_rate_reduction": 0.0,
      "all_controls_same_full_cohort_evaluator": true,
      "automatic_coverage": 0.0,
      "lesion_recall_delta_ci_low": -1.0,
      "overall_referral_rate": 1.0,
      "patient_macro_dice_delta_ci_low": -1.0,
      "positive_refer_counted_as_failure": true,
      "status": "NOT_ESTIMABLE_DUE_TO_INSUFFICIENT_PHASE1_EVIDENCE"
    },
    "candidate_pool_oracle_at_98pct_lesion_sensitivity": {
      "lesion_sensitivity": 0.98,
      "negative_view_fp_reduction_attainable": false,
      "status": "NOT_ESTIMABLE_DUE_TO_INSUFFICIENT_PHASE1_EVIDENCE"
    },
    "event_sufficiency": {
      "any_meta_fold_single_class": false,
      "confidence_intervals_stably_estimable": false,
      "fold_failures": [
        {
          "any_meta_fold_single_class": false,
          "effective_failure_events_sufficient": false,
          "reason": "UNSTABLE_THRESHOLD / NO_DECISION: lightweight_quality_regressor: {'status': 'UNSTABLE_THRESHOLD / NO_DECISION',
          'threshold': 0.005818983800356026, 'fold_thresholds': [{'heldout_meta_fold': 0, 'threshold': 0.005818983800356026,
          'training_fold_sensitivity': 0.9722222222222222, 'target_attainable': False}, {'heldout_meta_fold': 1, 'threshold':
          0.005818983800356026, 'training_fold_sensitivity': 0.972972972972973, 'target_attainable': False}, {'heldout_meta_fold': 2,
          'threshold': 0.005818983800356026, 'training_fold_sensitivity': 0.9622641509433962, 'target_attainable': False},
          {'heldout_meta_fold': 3, 'threshold': 0.3016642407532461, 'training_fold_sensitivity': 0.9821428571428571,
          'target_attainable': True}], 'fold_threshold_range': 0.2958452569528901, 'max_fold_threshold_range': 0.25,
          'oof_lesion_sensitivity': 0.9764705882352941, 'oof_patient_macro_normal_fp_rate': 0.8342394873644873, 'target_attainable':
          False, 'selection_source': 'leave_one_meta_fold_out_then_median_inner_meta_oof_only'}",
          "status": "NO_DECISION_INSUFFICIENT_EVIDENCE_PENDING_COMPLETE_FIVE_FOLDS",
          "threshold_unstable": true
        },
        {
          "any_meta_fold_single_class": false,
          "effective_failure_events_sufficient": false,
          "reason": "UNSTABLE_THRESHOLD / NO_DECISION: lightweight_quality_regressor: {'status': 'UNSTABLE_THRESHOLD / NO_DECISION',
          'threshold': 0.21075371050969569, 'fold_thresholds': [{'heldout_meta_fold': 0, 'threshold': 0.14537104498263126,
          'training_fold_sensitivity': 0.9859154929577465, 'target_attainable': True}, {'heldout_meta_fold': 1, 'threshold':
          0.14537104498263126, 'training_fold_sensitivity': 0.9848484848484849, 'target_attainable': True}, {'heldout_meta_fold': 2,
          'threshold': 0.41411142494413244, 'training_fold_sensitivity': 0.9852941176470589, 'target_attainable': True},
          {'heldout_meta_fold': 3, 'threshold': 0.2761363760367601, 'training_fold_sensitivity': 0.9838709677419355,
          'target_attainable': True}], 'fold_threshold_range': 0.2687403799615012, 'max_fold_threshold_range': 0.25,
          'oof_lesion_sensitivity': 0.9775280898876404, 'oof_patient_macro_normal_fp_rate': 0.6286546786546786, 'target_attainable':
          False, 'selection_source': 'leave_one_meta_fold_out_then_median_inner_meta_oof_only'}",
          "status": "NO_DECISION_INSUFFICIENT_EVIDENCE_PENDING_COMPLETE_FIVE_FOLDS",
          "threshold_unstable": true
        },
        {
          "any_meta_fold_single_class": false,
          "effective_failure_events_sufficient": false,
          "reason": "UNSTABLE_THRESHOLD / NO_DECISION: area_component_rule: {'status': 'UNSTABLE_THRESHOLD / NO_DECISION',
          'threshold': 0.38394535363088067, 'fold_thresholds': [{'heldout_meta_fold': 0, 'threshold': 0.4756303111058337,
          'training_fold_sensitivity': 0.9857142857142858, 'target_attainable': True}, {'heldout_meta_fold': 1, 'threshold':
          0.2922603961559277, 'training_fold_sensitivity': 0.984375, 'target_attainable': True}, {'heldout_meta_fold': 2,
          'threshold': 0.2922603961559277, 'training_fold_sensitivity': 0.9866666666666667, 'target_attainable': True},
          {'heldout_meta_fold': 3, 'threshold': 0.6557262142862044, 'training_fold_sensitivity': 0.9827586206896551,
          'target_attainable': True}], 'fold_threshold_range': 0.3634658181302767, 'max_fold_threshold_range': 0.25,
          'oof_lesion_sensitivity': 0.9775280898876404, 'oof_patient_macro_normal_fp_rate': 0.5903101528101528, 'target_attainable':
          False, 'selection_source': 'leave_one_meta_fold_out_then_median_inner_meta_oof_only'}",
          "status": "NO_DECISION_INSUFFICIENT_EVIDENCE_PENDING_COMPLETE_FIVE_FOLDS",
          "threshold_unstable": true
        },
        {
          "any_meta_fold_single_class": false,
          "effective_failure_events_sufficient": false,
          "reason": "UNSTABLE_THRESHOLD / NO_DECISION: lightweight_quality_regressor: {'status': 'UNSTABLE_THRESHOLD / NO_DECISION',
          'threshold': 0.16305705159157358, 'fold_thresholds': [{'heldout_meta_fold': 0, 'threshold': 0.16305705159157358,
          'training_fold_sensitivity': 0.9830508474576272, 'target_attainable': True}, {'heldout_meta_fold': 1, 'threshold':
          0.6023991711245025, 'training_fold_sensitivity': 0.9855072463768116, 'target_attainable': True}, {'heldout_meta_fold': 2,
          'threshold': 0.16305705159157358, 'training_fold_sensitivity': 0.9846153846153847, 'target_attainable': True},
          {'heldout_meta_fold': 3, 'threshold': 0.16305705159157358, 'training_fold_sensitivity': 0.9859154929577465,
          'target_attainable': True}], 'fold_threshold_range': 0.4393421195329289, 'max_fold_threshold_range': 0.25,
          'oof_lesion_sensitivity': 0.9886363636363636, 'oof_patient_macro_normal_fp_rate': 0.5917330447330447, 'target_attainable':
          True, 'selection_source': 'leave_one_meta_fold_out_then_median_inner_meta_oof_only'}",
          "status": "NO_DECISION_INSUFFICIENT_EVIDENCE_PENDING_COMPLETE_FIVE_FOLDS",
          "threshold_unstable": true
        }
      ],
      "max_fold_threshold_range": 1.0,
      "meta_fold_unique_patient_counts": {},
      "unique_patient_counts": {}
    },
    "phase1_completion": {
      "completed_outer_folds": [
        0,
        1,
        2,
        3,
        4
      ],
      "frozen_code_sha256_across_folds": true,
      "methods": [
        "B1",
        "Mask R-CNN",
        "B3",
        "detector_score",
        "sam_predicted_iou",
        "sam_stability",
        "jitter_variance",
        "area_component_rule",
        "lightweight_quality_regressor",
        "B5"
      ],
      "outer_folds": [
        0,
        1,
        2,
        3,
        4
      ],
      "outer_test_evaluations_per_patient": 1,
      "outer_test_used_for_route_or_threshold_selection": false,
      "pointrend_executed": false,
      "seed": 2027
    },
    "predicted_box_localization": {
      "metric": "patient_cluster_bootstrap_recall_at_1_fp_per_view",
      "recall_ci_high": 1.0,
      "recall_ci_low": 0.0,
      "status": "NOT_ESTIMABLE_DUE_TO_INSUFFICIENT_PHASE1_EVIDENCE"
    },
    "protocol_version": "2.3",
    "schema_version": 3,
    "simple_control_inner_meta_oof_ranking": {
      "controls": [
        "detector_score",
        "sam_predicted_iou",
        "sam_stability",
        "jitter_variance",
        "area_component_rule",
        "lightweight_quality_regressor"
      ],
      "selection_score_source": "PATIENT_GROUPED_META_OOF_ONLY",
      "status": "NOT_ESTIMABLE_DUE_TO_INSUFFICIENT_PHASE1_EVIDENCE",
      "strongest_control": "detector_score"
    }
  }

  ### PHASE1_COMPLETE.json

  {
    "completed_outer_folds": [
      0,
      1,
      2,
      3,
      4
    ],
    "folds": [
      {
        "code_tree_sha256": "47faa8eeaac7fe279efd08711586dce150f0b7ea795ca50ebeda01ce6d5c6323",
        "completed_at": "2026-07-18T13:14:09.395904+00:00",
        "config_sha256": "2d2bb53931cb84f047ec655354bbe9f402825f4209dc168fe45d89a52fe45cd8",
        "evaluation_patient_ids": [
          "ASSC",
          "CHVI",
          "FLBA",
          "KIFO",
          "VITR",
          "WAQU"
        ],
        "insufficient_evidence": true,
        "insufficient_evidence_path": "/workspace/ScreenBUS/server_bundle/runtime/output/phase1/fold_0/
        phase1_insufficient_evidence.json",
        "outer_fold": 0,
        "outer_test_used_for_route_or_threshold_selection": false,
        "pointrend_executed": false,
        "seed": 2027,
        "split_sha256": "621ba9aee0981e052b16f217126dca808f65436356d6a26a7b94c8eac499ccde",
        "status": "PHASE1_OUTER_FOLD_COMPLETE"
      },
      {
        "code_tree_sha256": "47faa8eeaac7fe279efd08711586dce150f0b7ea795ca50ebeda01ce6d5c6323",
        "completed_at": "2026-07-18T16:51:04.894207+00:00",
        "config_sha256": "2d2bb53931cb84f047ec655354bbe9f402825f4209dc168fe45d89a52fe45cd8",
        "evaluation_patient_ids": [
          "ANAT",
          "CHCO",
          "CODE",
          "COST",
          "DAPA",
          "OSCU",
          "SECH"
        ],
        "insufficient_evidence": false,
        "insufficient_evidence_path": null,
        "outer_fold": 1,
        "outer_test_used_for_route_or_threshold_selection": false,
        "pointrend_executed": false,
        "seed": 2027,
        "split_sha256": "b27390a734ea35d941729928d89ef07ef6270b43c8de8fc13db3adfc6b002c93",
        "status": "PHASE1_OUTER_FOLD_COMPLETE"
      },
      {
        "code_tree_sha256": "47faa8eeaac7fe279efd08711586dce150f0b7ea795ca50ebeda01ce6d5c6323",
        "completed_at": "2026-07-18T20:13:46.717075+00:00",
        "config_sha256": "2d2bb53931cb84f047ec655354bbe9f402825f4209dc168fe45d89a52fe45cd8",
        "evaluation_patient_ids": [
          "ALWI",
          "COVA",
          "LOTI",
          "NIRO",
          "STSP",
          "UNCU"
        ],
        "insufficient_evidence": true,
        "insufficient_evidence_path": "/workspace/ScreenBUS/server_bundle/runtime/output/phase1/fold_2/
        phase1_insufficient_evidence.json",
        "outer_fold": 2,
        "outer_test_used_for_route_or_threshold_selection": false,
        "pointrend_executed": false,
        "seed": 2027,
        "split_sha256": "23d0438f037be9b4745e1085c56d105de751476888c1a95d98522aa4daf2234b",
        "status": "PHASE1_OUTER_FOLD_COMPLETE"
      },
      {
        "code_tree_sha256": "47faa8eeaac7fe279efd08711586dce150f0b7ea795ca50ebeda01ce6d5c6323",
        "completed_at": "2026-07-18T23:36:46.681160+00:00",
        "config_sha256": "2d2bb53931cb84f047ec655354bbe9f402825f4209dc168fe45d89a52fe45cd8",
        "evaluation_patient_ids": [
          "CHSP",
          "FUHI",
          "HUBL",
          "PAGY",
          "PLBA",
          "TOCI"
        "status": "PHASE1_OUTER_FOLD_COMPLETE"
      },
      {
        "code_tree_sha256": "47faa8eeaac7fe279efd08711586dce150f0b7ea795ca50ebeda01ce6d5c6323",
        "completed_at": "2026-07-19T03:34:20.434685+00:00",
        "config_sha256": "2d2bb53931cb84f047ec655354bbe9f402825f4209dc168fe45d89a52fe45cd8",
        "evaluation_patient_ids": [
          "CAWI",
          "MENE",
          "ORPE",
          "POFR",
          "SHST",
          "SIBA"
        ],
        "insufficient_evidence": true,
        "insufficient_evidence_path": "/workspace/ScreenBUS/server_bundle/runtime/output/phase1/fold_4/
        phase1_insufficient_evidence.json",
        "outer_fold": 4,
        "outer_test_used_for_route_or_threshold_selection": false,
        "pointrend_executed": false,
        "seed": 2027,
        "split_sha256": "6c4e4a2d6cac2148f1909ef487409d4e04c1cfa892ca37ea2321a2c161b7547b",
        "status": "PHASE1_OUTER_FOLD_COMPLETE"
      }
    ],
    "g3_run": false,
    "phase1_report": "/workspace/ScreenBUS/server_bundle/runtime/output/phase1/PHASE1_FIVE_FOLD_REPORT.json",
    "phase1_report_sha256": "bf018bb336308058e928552ec9dc8be06ae2b9001ce5ffd00351f0fd824bd7be",
    "phase2_run": false,
    "protocol_version": "2.3",
    "schema_version": 3,
    "seed": 2027,
    "status": "PHASE1_FIVE_FOLD_ONE_SEED_COMPLETE_PENDING_G3"
  }

