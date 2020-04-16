load("@meru//:meru.bzl", "block", "sim_test")

sim_test(
    name = "test",
    top = "top_tb",
    top_file = "top_tb.sv",
    blocks = [":env"]
)

block(
    name = "env",
    vlog_files = [
        "verification_pack.sv",
        "generation_parameters.sv",
        "msg_sequence.sv",
        "verification_typedefs.sv",
        "coverage.sv",
        "reference_model.sv",
        "virtual_sequencer.sv",
        "virtual_sequence.sv",
        "environment.sv",
        "base_test.sv",
        "top_tb.sv",
    ]
    blocks = [
        "//avalon_st:avalon_st_if",
        "//avalon_st:avalon_st",
        "//general_scoreboard:general_scoreboard",
    ]
)
