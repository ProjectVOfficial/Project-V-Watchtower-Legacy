# Public Release Checklist

## Build

- [ ] TypeScript typecheck passes
- [ ] Vite production build passes
- [ ] Rust release build passes
- [ ] NSIS installer is generated
- [ ] MSI installer is generated
- [ ] Standalone / portable build is generated when applicable
- [ ] Application launches after installation
- [ ] Main dashboard loads
- [ ] Separate Project V windows open
- [ ] Uninstall behavior is tested
- [ ] Upgrade behavior is tested where applicable

## Security

- [ ] No `.env` files in public source
- [ ] No API keys
- [ ] No updater private key
- [ ] No certificate private key
- [ ] No personal research or local databases
- [ ] No private logs
- [ ] SHA-256 checksums generated
- [ ] Corresponding source manually inspected
- [ ] Security warning remains accurate
- [ ] Unsigned status is disclosed when applicable

## License, copyright, and attribution

- [ ] AGPL license included
- [ ] Corresponding source for the exact binary build is available
- [ ] Upstream notices preserved
- [ ] `NOTICE.md` included
- [ ] Material Project V modifications are identified
- [ ] Third-party notices reviewed
- [ ] Provider attribution reviewed
- [ ] Project V is not represented as official World Monitor upstream
- [ ] Trademarks and assets reviewed
- [ ] No additional restriction conflicts with AGPL rights for covered code

## Documentation

- [ ] README reviewed
- [ ] Installation guide reviewed
- [ ] White paper reviewed
- [ ] Security policy reviewed
- [ ] Privacy notes reviewed
- [ ] Release notes reviewed
- [ ] Changelog reviewed
- [ ] Known limitations reviewed
- [ ] Support instructions reviewed
- [ ] Upstream/license notice reviewed

## GitHub

- [ ] Repository owner is `ProjectVOfficial`
- [ ] Repository visibility is correct
- [ ] Draft release created
- [ ] Installer / executable assets attached
- [ ] Corresponding source attached or otherwise provided in a clearly compliant release path
- [ ] Checksums attached
- [ ] Release notes link to license and upstream notice
- [ ] Downloaded assets match checksums
- [ ] Draft reviewed on GitHub
- [ ] Release published intentionally
