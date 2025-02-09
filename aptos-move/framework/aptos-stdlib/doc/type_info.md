
<a name="0x1_type_info"></a>

# Module `0x1::type_info`



-  [Struct `TypeInfo`](#0x1_type_info_TypeInfo)
-  [Function `account_address`](#0x1_type_info_account_address)
-  [Function `module_name`](#0x1_type_info_module_name)
-  [Function `struct_name`](#0x1_type_info_struct_name)
-  [Function `type_of`](#0x1_type_info_type_of)
-  [Function `type_name`](#0x1_type_info_type_name)
-  [Function `verify_type_of`](#0x1_type_info_verify_type_of)
-  [Function `verify_type_of_generic`](#0x1_type_info_verify_type_of_generic)


<pre><code><b>use</b> <a href="../../move-stdlib/doc/string.md#0x1_string">0x1::string</a>;
</code></pre>



<a name="0x1_type_info_TypeInfo"></a>

## Struct `TypeInfo`



<pre><code><b>struct</b> <a href="type_info.md#0x1_type_info_TypeInfo">TypeInfo</a> <b>has</b> <b>copy</b>, drop, store
</code></pre>



<details>
<summary>Fields</summary>


<dl>
<dt>
<code>account_address: <b>address</b></code>
</dt>
<dd>

</dd>
<dt>
<code>module_name: <a href="../../move-stdlib/doc/vector.md#0x1_vector">vector</a>&lt;u8&gt;</code>
</dt>
<dd>

</dd>
<dt>
<code>struct_name: <a href="../../move-stdlib/doc/vector.md#0x1_vector">vector</a>&lt;u8&gt;</code>
</dt>
<dd>

</dd>
</dl>


</details>

<a name="0x1_type_info_account_address"></a>

## Function `account_address`



<pre><code><b>public</b> <b>fun</b> <a href="type_info.md#0x1_type_info_account_address">account_address</a>(<a href="type_info.md#0x1_type_info">type_info</a>: &<a href="type_info.md#0x1_type_info_TypeInfo">type_info::TypeInfo</a>): <b>address</b>
</code></pre>



<details>
<summary>Implementation</summary>


<pre><code><b>public</b> <b>fun</b> <a href="type_info.md#0x1_type_info_account_address">account_address</a>(<a href="type_info.md#0x1_type_info">type_info</a>: &<a href="type_info.md#0x1_type_info_TypeInfo">TypeInfo</a>): <b>address</b> {
    <a href="type_info.md#0x1_type_info">type_info</a>.account_address
}
</code></pre>



</details>

<a name="0x1_type_info_module_name"></a>

## Function `module_name`



<pre><code><b>public</b> <b>fun</b> <a href="type_info.md#0x1_type_info_module_name">module_name</a>(<a href="type_info.md#0x1_type_info">type_info</a>: &<a href="type_info.md#0x1_type_info_TypeInfo">type_info::TypeInfo</a>): <a href="../../move-stdlib/doc/vector.md#0x1_vector">vector</a>&lt;u8&gt;
</code></pre>



<details>
<summary>Implementation</summary>


<pre><code><b>public</b> <b>fun</b> <a href="type_info.md#0x1_type_info_module_name">module_name</a>(<a href="type_info.md#0x1_type_info">type_info</a>: &<a href="type_info.md#0x1_type_info_TypeInfo">TypeInfo</a>): <a href="../../move-stdlib/doc/vector.md#0x1_vector">vector</a>&lt;u8&gt; {
    <a href="type_info.md#0x1_type_info">type_info</a>.module_name
}
</code></pre>



</details>

<a name="0x1_type_info_struct_name"></a>

## Function `struct_name`



<pre><code><b>public</b> <b>fun</b> <a href="type_info.md#0x1_type_info_struct_name">struct_name</a>(<a href="type_info.md#0x1_type_info">type_info</a>: &<a href="type_info.md#0x1_type_info_TypeInfo">type_info::TypeInfo</a>): <a href="../../move-stdlib/doc/vector.md#0x1_vector">vector</a>&lt;u8&gt;
</code></pre>



<details>
<summary>Implementation</summary>


<pre><code><b>public</b> <b>fun</b> <a href="type_info.md#0x1_type_info_struct_name">struct_name</a>(<a href="type_info.md#0x1_type_info">type_info</a>: &<a href="type_info.md#0x1_type_info_TypeInfo">TypeInfo</a>): <a href="../../move-stdlib/doc/vector.md#0x1_vector">vector</a>&lt;u8&gt; {
    <a href="type_info.md#0x1_type_info">type_info</a>.struct_name
}
</code></pre>



</details>

<a name="0x1_type_info_type_of"></a>

## Function `type_of`



<pre><code><b>public</b> <b>fun</b> <a href="type_info.md#0x1_type_info_type_of">type_of</a>&lt;T&gt;(): <a href="type_info.md#0x1_type_info_TypeInfo">type_info::TypeInfo</a>
</code></pre>



<details>
<summary>Implementation</summary>


<pre><code><b>public</b> <b>native</b> <b>fun</b> <a href="type_info.md#0x1_type_info_type_of">type_of</a>&lt;T&gt;(): <a href="type_info.md#0x1_type_info_TypeInfo">TypeInfo</a>;
</code></pre>



</details>

<a name="0x1_type_info_type_name"></a>

## Function `type_name`



<pre><code><b>public</b> <b>fun</b> <a href="type_info.md#0x1_type_info_type_name">type_name</a>&lt;T&gt;(): <a href="../../move-stdlib/doc/string.md#0x1_string_String">string::String</a>
</code></pre>



<details>
<summary>Implementation</summary>


<pre><code><b>public</b> <b>native</b> <b>fun</b> <a href="type_info.md#0x1_type_info_type_name">type_name</a>&lt;T&gt;(): <a href="../../move-stdlib/doc/string.md#0x1_string_String">string::String</a>;
</code></pre>



</details>

<a name="0x1_type_info_verify_type_of"></a>

## Function `verify_type_of`



<pre><code><b>fun</b> <a href="type_info.md#0x1_type_info_verify_type_of">verify_type_of</a>()
</code></pre>



<details>
<summary>Implementation</summary>


<pre><code><b>fun</b> <a href="type_info.md#0x1_type_info_verify_type_of">verify_type_of</a>() {
    <b>let</b> <a href="type_info.md#0x1_type_info">type_info</a> = <a href="type_info.md#0x1_type_info_type_of">type_of</a>&lt;<a href="type_info.md#0x1_type_info_TypeInfo">TypeInfo</a>&gt;();
    <b>let</b> account_address = <a href="type_info.md#0x1_type_info_account_address">account_address</a>(&<a href="type_info.md#0x1_type_info">type_info</a>);
    <b>let</b> module_name = <a href="type_info.md#0x1_type_info_module_name">module_name</a>(&<a href="type_info.md#0x1_type_info">type_info</a>);
    <b>let</b> struct_name = <a href="type_info.md#0x1_type_info_struct_name">struct_name</a>(&<a href="type_info.md#0x1_type_info">type_info</a>);
    <b>spec</b> {
        <b>assert</b> account_address == @aptos_std;
        <b>assert</b> module_name == b"<a href="type_info.md#0x1_type_info">type_info</a>";
        <b>assert</b> struct_name == b"<a href="type_info.md#0x1_type_info_TypeInfo">TypeInfo</a>";
    };
}
</code></pre>



</details>

<a name="0x1_type_info_verify_type_of_generic"></a>

## Function `verify_type_of_generic`



<pre><code><b>fun</b> <a href="type_info.md#0x1_type_info_verify_type_of_generic">verify_type_of_generic</a>&lt;T&gt;()
</code></pre>



<details>
<summary>Implementation</summary>


<pre><code><b>fun</b> <a href="type_info.md#0x1_type_info_verify_type_of_generic">verify_type_of_generic</a>&lt;T&gt;() {
    <b>let</b> <a href="type_info.md#0x1_type_info">type_info</a> = <a href="type_info.md#0x1_type_info_type_of">type_of</a>&lt;T&gt;();
    <b>let</b> account_address = <a href="type_info.md#0x1_type_info_account_address">account_address</a>(&<a href="type_info.md#0x1_type_info">type_info</a>);
    <b>let</b> module_name = <a href="type_info.md#0x1_type_info_module_name">module_name</a>(&<a href="type_info.md#0x1_type_info">type_info</a>);
    <b>let</b> struct_name = <a href="type_info.md#0x1_type_info_struct_name">struct_name</a>(&<a href="type_info.md#0x1_type_info">type_info</a>);
    <b>spec</b> {
        <b>assert</b> account_address == <a href="type_info.md#0x1_type_info_type_of">type_of</a>&lt;T&gt;().account_address;
        <b>assert</b> module_name == <a href="type_info.md#0x1_type_info_type_of">type_of</a>&lt;T&gt;().module_name;
        <b>assert</b> struct_name == <a href="type_info.md#0x1_type_info_type_of">type_of</a>&lt;T&gt;().struct_name;
    };
}
</code></pre>



</details>


[move-book]: https://move-language.github.io/move/introduction.html
