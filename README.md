# windows-config
Just some useful windows commands and tweaks.

You may also be interested in my [windows-registry Repository](https://github.com/EnnoxHD/windows-registry).

---

## Disclaimer
>THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

For more Information see [License](./LICENSE).

---

## Disable hibernate energy state
1. Open `cmd` as an administrator
1. `powercfg -h off`

## Disable Windows Recovery

### Disable the recovery functions in the Recovery Environment
1. Open `cmd` as an administrator
1. `ReAgentc.exe /disable`
1. Check the status with: `ReAgentc.exe /info`
1. Reenable with: `ReAgentc.exe /enable`

### Disable the entire Recovery Environment
1. Open `cmd` as an administrator
1. `bcdedit.exe /set recoveryenabled NO`
1. Reenable with: `bcdedit.exe /set recoveryenabled YES`
