cmake_minimum_required(VERSION 3.5)
project(os_ass4)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11")

set(SOURCE_FILES
    asm.h
    bio.c
    bootmain.c
    buf.h
    cat.c
    console.c
    date.h
    defs.h
    echo.c
    elf.h
    exec.c
    fcntl.h
    file.c
    file.h
    forktest.c
    fs.c
    fs.h
    grep.c
    ide.c
    init.c
    ioapic.c
    kalloc.c
    kbd.c
    kbd.h
    kill.c
    lapic.c
    ln.c
    log.c
    ls.c
    main.c
    mbr.h
    memide.c
    memlayout.h
    mkdir.c
    mkfs.c
    mmu.h
    mp.c
    mp.h
    param.h
    picirq.c
    pipe.c
    printf.c
    proc.c
    proc.h
    rm.c
    sh.c
    spinlock.c
    spinlock.h
    stat.h
    stressfs.c
    string.c
    syscall.c
    syscall.h
    sysfile.c
    sysproc.c
    timer.c
    trap.c
    traps.h
    types.h
    uart.c
    ulib.c
    umalloc.c
    user.h
    usertests.c
    vm.c
    wc.c
    x86.h
    zombie.c)

include_directories(.)

add_executable(os_ass4 ${SOURCE_FILES})