# remote-solveit-kernel

Minimal remote kernel environment for Solveit handoff.

## Remote setup and launch

From a fresh clone:

```bash
uv sync
```

Then launch the remote kernel with the transferred connection file:

```bash
uv run --no-sync ipyku-launcher -f /tmp/remote_kernel_connection.json
```

Equivalent direct venv command:

```bash
.venv/bin/ipyku-launcher -f /tmp/remote_kernel_connection.json
```

Use `ipyku-launcher` rather than `python -m ipykernel_launcher` when the kernel
needs `ipyk_unlock`.
