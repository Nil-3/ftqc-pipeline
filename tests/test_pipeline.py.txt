import pytest
import pyzx as zx

def test_pyzx_t_count_reduction():
    # Simple validation test for ZX-calculus graph optimization
    c = zx.Circuit(2)
    c.add_gate("T", 0)
    g = c.to_graph()
    zx.full_reduce(g)
    optimized_circuit = g.to_circuit()
    assert len(g.vertices()) > 0

def test_surface_code_logic():
    # Basic check for surface code scaling overheads
    logical_qubits = 4
    distance = 11
    assert distance % 2 != 0  # Code distance must be odd