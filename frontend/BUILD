files(
    name = "project-files",
    sources = [
        "src/**",
        "public/**",
        "package.json",
        "tsconfig.json",
        "next.config.js",
        ".eslintrc.json",
    ],
)

package_json(
    name = "package-json",
    dependencies = [
        ":project-files",
        "//:root-files",
        "//libs/types:files",
    ],
    scripts = [
        node_build_script(
            entry_point = "build",
            output_directories = ["build/.next"],
        ),
    ],
)
