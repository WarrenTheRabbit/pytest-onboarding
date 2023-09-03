#### Context
The hierachies within the public API should be visualised.

#### Input 
<li><p><a class="reference internal" href="#constants" id="id4">Constants</a></p>
<ul>
<li><p><a class="reference internal" href="#pytest-version" id="id5">pytest.__version__</a></p></li>
<li><p><a class="reference internal" href="#pytest-version-tuple" id="id6">pytest.version_tuple</a></p></li>
</ul>
</li>
<li><p><a class="reference internal" href="#functions" id="id7">Functions</a></p>
<ul>
<li><p><a class="reference internal" href="#pytest-approx" id="id8">pytest.approx</a></p></li>
<li><p><a class="reference internal" href="#pytest-fail" id="id9">pytest.fail</a></p></li>
<li><p><a class="reference internal" href="#pytest-skip" id="id10">pytest.skip</a></p></li>
<li><p><a class="reference internal" href="#pytest-importorskip" id="id11">pytest.importorskip</a></p></li>
<li><p><a class="reference internal" href="#pytest-xfail" id="id12">pytest.xfail</a></p></li>
<li><p><a class="reference internal" href="#pytest-exit" id="id13">pytest.exit</a></p></li>
<li><p><a class="reference internal" href="#pytest-main" id="id14">pytest.main</a></p></li>
<li><p><a class="reference internal" href="#pytest-param" id="id15">pytest.param</a></p></li>
<li><p><a class="reference internal" href="#pytest-raises" id="id16">pytest.raises</a></p></li>
<li><p><a class="reference internal" href="#pytest-deprecated-call" id="id17">pytest.deprecated_call</a></p></li>
<li><p><a class="reference internal" href="#pytest-register-assert-rewrite" id="id18">pytest.register_assert_rewrite</a></p></li>
<li><p><a class="reference internal" href="#pytest-warns" id="id19">pytest.warns</a></p></li>
<li><p><a class="reference internal" href="#pytest-freeze-includes" id="id20">pytest.freeze_includes</a></p></li>
</ul>
</li>
<li><p><a class="reference internal" href="#marks" id="id21">Marks</a></p>
<ul>
<li><p><a class="reference internal" href="#pytest-mark-filterwarnings" id="id22">pytest.mark.filterwarnings</a></p></li>
<li><p><a class="reference internal" href="#pytest-mark-parametrize" id="id23">pytest.mark.parametrize</a></p></li>
<li><p><a class="reference internal" href="#pytest-mark-skip" id="id24">pytest.mark.skip</a></p></li>
<li><p><a class="reference internal" href="#pytest-mark-skipif" id="id25">pytest.mark.skipif</a></p></li>
<li><p><a class="reference internal" href="#pytest-mark-usefixtures" id="id26">pytest.mark.usefixtures</a></p></li>
<li><p><a class="reference internal" href="#pytest-mark-xfail" id="id27">pytest.mark.xfail</a></p></li>
<li><p><a class="reference internal" href="#custom-marks" id="id28">Custom marks</a></p></li>
</ul>
</li>
<li><p><a class="reference internal" href="#fixtures" id="id29">Fixtures</a></p>
<ul>
<li><p><a class="reference internal" href="#pytest-fixture" id="id30">&#64;pytest.fixture</a></p></li>
<li><p><a class="reference internal" href="#config-cache" id="id31">config.cache</a></p></li>
<li><p><a class="reference internal" href="#capsys" id="id32">capsys</a></p></li>
<li><p><a class="reference internal" href="#capsysbinary" id="id33">capsysbinary</a></p></li>
<li><p><a class="reference internal" href="#capfd" id="id34">capfd</a></p></li>
<li><p><a class="reference internal" href="#capfdbinary" id="id35">capfdbinary</a></p></li>
<li><p><a class="reference internal" href="#doctest-namespace" id="id36">doctest_namespace</a></p></li>
<li><p><a class="reference internal" href="#request" id="id37">request</a></p></li>
<li><p><a class="reference internal" href="#pytestconfig" id="id38">pytestconfig</a></p></li>
<li><p><a class="reference internal" href="#record-property" id="id39">record_property</a></p></li>
<li><p><a class="reference internal" href="#record-testsuite-property" id="id40">record_testsuite_property</a></p></li>
<li><p><a class="reference internal" href="#caplog" id="id41">caplog</a></p></li>
<li><p><a class="reference internal" href="#monkeypatch" id="id42">monkeypatch</a></p></li>
<li><p><a class="reference internal" href="#pytester" id="id43">pytester</a></p></li>
<li><p><a class="reference internal" href="#testdir" id="id44">testdir</a></p></li>
<li><p><a class="reference internal" href="#recwarn" id="id45">recwarn</a></p></li>
<li><p><a class="reference internal" href="#tmp-path" id="id46">tmp_path</a></p></li>
<li><p><a class="reference internal" href="#tmp-path-factory" id="id47">tmp_path_factory</a></p></li>
<li><p><a class="reference internal" href="#tmpdir" id="id48">tmpdir</a></p></li>
<li><p><a class="reference internal" href="#tmpdir-factory" id="id49">tmpdir_factory</a></p></li>
</ul>
</li>
<li><p><a class="reference internal" href="#hooks" id="id50">Hooks</a></p>
<ul>
<li><p><a class="reference internal" href="#bootstrapping-hooks" id="id51">Bootstrapping hooks</a></p></li>
<li><p><a class="reference internal" href="#initialization-hooks" id="id52">Initialization hooks</a></p></li>
<li><p><a class="reference internal" href="#collection-hooks" id="id53">Collection hooks</a></p></li>
<li><p><a class="reference internal" href="#test-running-runtest-hooks" id="id54">Test running (runtest) hooks</a></p></li>
<li><p><a class="reference internal" href="#reporting-hooks" id="id55">Reporting hooks</a></p></li>
<li><p><a class="reference internal" href="#debugging-interaction-hooks" id="id56">Debugging/Interaction hooks</a></p></li>
</ul>
</li>
<li><p><a class="reference internal" href="#objects" id="id57">Objects</a></p>
<ul>
<li><p><a class="reference internal" href="#callinfo" id="id58">CallInfo</a></p></li>
<li><p><a class="reference internal" href="#class" id="id59">Class</a></p></li>
<li><p><a class="reference internal" href="#collector" id="id60">Collector</a></p></li>
<li><p><a class="reference internal" href="#collectreport" id="id61">CollectReport</a></p></li>
<li><p><a class="reference internal" href="#config" id="id62">Config</a></p></li>
<li><p><a class="reference internal" href="#exceptioninfo" id="id63">ExceptionInfo</a></p></li>
<li><p><a class="reference internal" href="#exitcode" id="id64">ExitCode</a></p></li>
<li><p><a class="reference internal" href="#file" id="id65">File</a></p></li>
<li><p><a class="reference internal" href="#fixturedef" id="id66">FixtureDef</a></p></li>
<li><p><a class="reference internal" href="#fscollector" id="id67">FSCollector</a></p></li>
<li><p><a class="reference internal" href="#function" id="id68">Function</a></p></li>
<li><p><a class="reference internal" href="#functiondefinition" id="id69">FunctionDefinition</a></p></li>
<li><p><a class="reference internal" href="#item" id="id70">Item</a></p></li>
<li><p><a class="reference internal" href="#markdecorator" id="id71">MarkDecorator</a></p></li>
<li><p><a class="reference internal" href="#markgenerator" id="id72">MarkGenerator</a></p></li>
<li><p><a class="reference internal" href="#mark" id="id73">Mark</a></p></li>
<li><p><a class="reference internal" href="#metafunc" id="id74">Metafunc</a></p></li>
<li><p><a class="reference internal" href="#module" id="id75">Module</a></p></li>
<li><p><a class="reference internal" href="#node" id="id76">Node</a></p></li>
<li><p><a class="reference internal" href="#parser" id="id77">Parser</a></p></li>
<li><p><a class="reference internal" href="#optiongroup" id="id78">OptionGroup</a></p></li>
<li><p><a class="reference internal" href="#pytestpluginmanager" id="id79">PytestPluginManager</a></p></li>
<li><p><a class="reference internal" href="#session" id="id80">Session</a></p></li>
<li><p><a class="reference internal" href="#testreport" id="id81">TestReport</a></p></li>
<li><p><a class="reference internal" href="#result" id="id82">_Result</a></p></li>
<li><p><a class="reference internal" href="#stash" id="id83">Stash</a></p></li>
</ul>
</li>
<li><p><a class="reference internal" href="#global-variables" id="id84">Global Variables</a></p></li>
<li><p><a class="reference internal" href="#environment-variables" id="id85">Environment Variables</a></p></li>
<li><p><a class="reference internal" href="#exceptions" id="id86">Exceptions</a></p></li>
<li><p><a class="reference internal" href="#warnings" id="id87">Warnings</a></p></li>
<li><p><a class="reference internal" href="#configuration-options" id="id88">Configuration Options</a></p></li>
<li><p><a class="reference internal" href="#command-line-flags" id="id89">Command-line Flags</a></p></li>

#### Output

Constants
    pytest.__version__
    pytest.version_tuple
Functions
    pytest.approx
    pytest.fail
    pytest.skip
    pytest.importorskip
    pytest.xfail
    pytest.exit
    pytest.main
    pytest.param
    pytest.raises
    pytest.deprecated_call
    pytest.register_assert_rewrite
    pytest.warns
    pytest.freeze_includes
Marks
    pytest.mark.filterwarnings
    pytest.mark.parametrize
    pytest.mark.skip
    pytest.mark.skipif
    pytest.mark.usefixtures
    pytest.mark.xfail
    Custom marks
Fixtures
    pytest.fixture
    config.cache
    capsys
    capsysbinary
    capfd
    capfdbinary
    doctest_namespace
    request
    pytestconfig
    record_property
    record_testsuite_property
    caplog
    monkeypatch
    pytester
    testdir
    recwarn
    tmp_path
    tmp_path_factory
    tmpdir
    tmpdir_factory
Hooks
    Bootstrapping hooks
    Initialization hooks
    Collection hooks
    Test running (runtest) hooks
    Reporting hooks
    Debugging/Interaction hooks
Objects
    CallInfo
    Class
    Collector
    CollectReport
    Config
    ExceptionInfo
    ExitCode
    File
    FixtureDef
    FSCollector
    Function
    FunctionDefinition
    Item
    MarkDecorator
    MarkGenerator
    Mark
    Metafunc
    Module
    Node
    Parser
    OptionGroup
    PytestPluginManager
    Session
    TestReport
    _Result
    Stash
    Global Variables
    Environment Variables
    Exceptions
    Warnings
    Configuration Options
    Command-line Flags